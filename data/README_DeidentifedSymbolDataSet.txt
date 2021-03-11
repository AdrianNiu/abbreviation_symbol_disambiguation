README:: De-identified Data Set, Symbols 
Version 1 (October 30, 2012)
Contact information: 
	Natural Language Processing/Information Extraction (NLP/IE) Program 
	Email: nlp-ie@umn.edu

---------------------------------------
Among the most frequently occurring symbols in clinical text, four common non-alphanumeric symbols ('+', '-', '/', and '#') were selected. For each, 1000 instances were de-identified and the senses (meanings) were manually annotated and are available for researchers. 

Reference of original study:
Automated non-alphanumeric symbol resolution in clinical texts. 
Moon S, Pakhomov S, Ryan J, Melton GB. 
AMIA Annu Symp Proc. 2011;2011:979-86. Epub 2011 Oct 22. 
PubMed PMID: 22195157; PubMed Central PMCID: PMC3243158.

Samples were de-identified using the safe harbor method. The basic format of identification codes is as _%#IDENTIFIER#%_ in data. Identifiers were replaced with the following identification codes:

Identifiers 1: Name
Identification codes: _%#NAME#%_

Identifiers 2: Street address (Geographic subdivisions)
Identification codes: _%#STREET#%_

Identifiers 3: City (Geographic subdivisions)
Identification codes: _%#CITY#%_

Identifiers 4: County (Geographic subdivisions)
Identification codes: _%#COUNTY#%_

Identifiers 5: Precinct (Geographic subdivisions)
Identification codes: _%#PRECINCT#%_

Identifiers 6: All geographic subdivisions smaller than a State (Geographic subdivisions)
Identification codes: _%#ADDRESS#%_

Identifiers 7: Zip code (Geographic subdivisions), The geographic unit formed by combining all zip codes with the same three initial digits contains more than 20,000 people
Identification codes: 55455 => _%#55400#%_

Identifiers 8: Zip code (Geographic subdivisions), All such geographic units containing 20,000 or fewer people
Identification codes: _%#00000#%_

Identifiers 9: Dates for under 89 (keep real year), All elements of dates (except year) for dates directly related to an individual, including birth date, admission date, discharge date, date of death
Identification codes: 02/07/2000 => _%#DDMM2000#%_ 
Identification codes: Feb, 07, 2000 => _%#MM#%_, _%#DD#%_, _%#2000#%_
Identification codes: 10/17 => _%#MMDD#%_

Identifiers 10: Dates for over 89
Identification codes: _%#DDMM1914#%_
Identification codes: Feb, 07, 1997 => _%#MM#%_, _%#DD#%_, _%#1914#%_

Identifiers 11: Telephone numbers
Identification codes: _%#TEL#%_

Identifiers 12: Fax numbers
Identification codes: _%#FAX#%_

Identifiers 13: Electronic mail addresses
Identification codes: _%#EMAIL#%_

Identifiers 14: Social security numbers
Identification codes: _%#SSN#%_

Identifiers 15: Medical record numbers
Identification codes: _%#MRN#%_

Identifiers 16: Health plan beneficiary numbers
Identification codes: _%#HPBN#%_

Identifiers 17: Account numbers
Identification codes: _%#ACCOUNTN#%_

Identifiers 18: Certificate/license numbers
Identification codes: _%#LN#%_

Identifiers 19: Vehicle identifiers and serial numbers, including license plate numbers
Identification codes: _%#VN#%_

Identifiers 20: Device
Identification codes: _%#DEVICE#%_

The de-identified symbol sentence data set pipe delimitated '|'. All whitespaces in sentences were replaced with spaces.
Column 1: The targeted symbol
Column 2: Sense, the meaning of the targeted symbol
Column 3: The position of the targeted symbol in the given sentence. The sentence starts from position 0.
Column 4: De-identified sample including the targeted symbol 