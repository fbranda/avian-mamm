# AVIAN-MAMM: A Global Open Access Dataset of Reported Avian Flu Events in Mammals


## About this repository <a name="AboutthisRepository"></a>

This is the public repository of the AVIAN-MAMM Dataset and related
documentation. <br>

This repository contains: <br>

**<code>latest-outbreaks-mammals.csv</code>**: This file contains the **raw data**
of the AVIAN-MAMM Dataset, reporting the latest information available on
avian flu events in animals. <br>

**<code>avian-mamm-visualization.Rmd</code>**: This Markdown file contains
the **code** to explore, describe, and visualize the dataset. <br>

**<code>Contributing.md</code>**: This file provides guidelines for
contributing to the project: suggesting changes to the data or to the
code, submitting new data, and contributing to the code.<br>

**<code>avian-mamm-PDF-archives</code>**: For each avian flu event
recorded in the dataset, a copy of the report used as primary information source is saved in this folder. 
Each report was downloaded as a .pdf file. <br>  

**<code>sequences</code>**: Genetic sequences made available by APHIS National Veterinary Services Laboratories from the U.S. influenza virus H5N1 clade 2.3.4.4b, recently found in samples associated with the ongoing highly pathogenic avian influenza (HPAI) outbreak in poultry and wild birds and the recent H5N1 event in dairy cattle.

The [AVIAN-MAMM Map](https://tinyurl.com/avianflu-mammals-map) provides
interactive visualizations of the dynamic version of the dataset. <br>

## About the Data <a name="Data"></a>

### Data sources

Information has been collected from the World Animal Health Information
System [WAHIS](https://wahis.woah.org/) of the World Organisation for
Animal Health ([WOAH](https://wahis.woah.org/#/home), formerly OIE).
<br>

[WAHIS](https://wahis.woah.org/) is a Web-based computer system that
processes data on animal diseases in real-time. WAHIS data reflects the
information gathered by the Veterinary Services from WOAH Members and
non-Members Countries and Territories on WOAH-listed diseases in
domestic animals and wildlife, as well as on emerging and zoonotic
diseases. The detection of infection with SARS-CoV-2 in animals meets
the criteria for reporting to the World Animal Health Organisation
(WOAH) as an emerging infection in accordance with the WOAH Terrestrial
Animal Health Code. Only authorized users, i.e. the Delegates of WOAH
Member Countries and their authorised representatives, can enter data
into the WAHIS platform to notify the WOAH of relevant animal disease
information. All information are publicly accessible on the
[WAHIS](https://wahis.woah.org/#/events) interface. <br>
<br>

### Data collection process

Data on each avian flu event in mammals was collected and entered
manually in a .csv file. <br>

### Field dictionary

<code>url_event</code>: Link to the online WAHIS source to summarize the event.<br>  

<code>url_pdf</code>: Link to the WAHIS report to document the event. <br>

<code>report_id</code>: Unique identifier for the report, as
provided by the WAHIS report. Also corresponds to the name of the PDF
file describing the event in the <code>avian-mamm-PDF-archives</code>
folder. <br>

<code>report_date</code>: When the avian flu event was reported by the WAHIS. <br>

<code>event_id</code>: Unique identifier for each unique event of avian flu
infection/exposure in mammal(s). <br>

<code>genotype_serotype_subtype</code>: Avian flu genotype/senotype/subtype name<br>

<code>test_name_1</code>: First type of laboratory test performed to detect infection with (presence of the virus is evidenced) or exposure to (presence of antibodies is evidenced) avian flu. <br>

<code>laboratory_name_1</code>: Name of laboratory that performed <code>test_name_1</code><br>

<code>first_result_date_1</code>: First result of <code>test_name_1</code><br>

<code>last_result_date_1</code>: Final result of <code>test_name_1</code><br>

<code>result_1</code>: Outcome of of <code>test_name_1</code><br>

<code>test_name_2</code>: Second type of laboratory test performed to detect infection with (presence of the virus is evidenced) or exposure to (presence of antibodies is evidenced) avian flu. <br>

<code>laboratory_name_2</code>: Name of laboratory that performed <code>test_name_2</code><br>

<code>first_result_date_2</code>: First result of <code>test_name_2</code><br>

<code>last_result_date_2</code>: Final result of <code>test_name_2</code><br>

<code>result_2</code>: Outcome of of <code>test_name_2</code><br>

<code>test_name_3</code>: Third type of laboratory test performed to detect infection with (presence of the virus is evidenced) or exposure to (presence of antibodies is evidenced) avian flu. <br>

<code>laboratory_name_3</code>: Name of laboratory that performed <code>test_name_3</code><br>

<code>first_result_date_3</code>: First result of <code>test_name_3</code><br>

<code>last_result_date_3</code>: Final result of <code>test_name_3</code><br>

<code>result_3</code>: Outcome of of <code>test_name_3</code><br>

<code>label_id</code>: Unique identifier of an outbreak.<br>

<code>outbreak_reference</code>: Unique identifier of an outbreak. If outbreak_reference = NA,  <br>

<code>start_date_outbreak</code>: Date of start of an outbreak.<br>

<code>end_date_outbreak</code>: Date of end of the outbreak.<br>

<code>country_name</code>: Name of the country where the avian flu event was reported.<br>

<code>country_iso3_letter</code>: Three-letter ISO country code for the country where the avian flu event was reported.<br>

<code>country_iso3_digit</code>: Three-digit ISO country code for the country where the avian flu event was reported.<br>

<code>first_administrative_division</code>: Name of the first administrative level of the geographical area where the avian influenza event was reported.<br>

<code>second_administrative_division</code>: Name of the second administrative level of the geographical area where the avian influenza event was reported.<br>

<code>third_administrative_division</code>: Name of the third administrative level of the geographical area where the avian influenza event was reported.<br>

<code>location</code>: Name of the location where the avian flu event was reported.<br>

<code>latitude</code>: Approximate latitude of the location where the avian flu event was reported.<br>

<code>longitude</code>: Approximate longitude of the location where the avian flu event was reported. <br>

<code>species</code>: The species name of a mammal host.  <br>

<code>typology_of_animal</code>: The category name of a mammal host. Pre-defined string values are: *wild* = a mammal species that exists and lives in its natural habitat; *domestic*: a mammal species that has been selectively bred and raised by humans for various purposes, such as companionship, work, agriculture, or other human needs.  <br>

<code>total_susceptible</code>: Reported number of susceptible mammal(s) of the same species in the event. <br>

<code>total_cases</code>: Reported number of mammal(s) tested positive for avian flu in the event. <br>

<code>total_deaths</code>: Reported number of direct and indirect death(s) related to the event. If death is not reported, number_deaths = NA.<br>

<code>total_killed_and_disposed_of</code>: Reported number of direct death(s) related to the event. If death is not reported, total_killed_and_disposed_of = NA.<br>

<code>total_slaughtered_killed_for_commercial_use</code>: Reported number of direct death(s) for commercial use related to the event. If death is not reported, total_slaughtered_killed_for_commercial_use = NA.<br>

<code>total_vaccinated</code>: Reported number of animal(s) vaccinated for avian flu in the event. <br> If death is not reported, total_slaughtered_killed_for_commercial_use = NA.<br>


<code>epidemiological_unit</code>: The epidemiological unit considered to describe the event. Possible pre-defined string values are: *zoo* = a group of mammals housed/living together (excluding farm animals); *farm*: a group of mammals belonging to the same species and bred for commercial purposes. <br>
 

<code>detailed_characterisation</code>: Description of the technical details of an outbreak (e.g., clade name)<br>  

<code>affected_population_description</code>: Description of the affected population (e.g., Animal with symptoms died shortly after discovery. HPAI H5N1 was detected in a Red fox (vulpes vulpes) found dead).<br>  

<code>control_measures</code>: Main intervention(s) implemented to mitigate further spread of the virus.<br>  

<code>outcome</code>: Issue of the avian flu infection (or exposure). If <code>total_cases</code> = <code>total_deaths</code>: "death"; If <code>total_cases</code> = <code>total_killed_and_disposed_of</code>: "death"; If <code>total_cases</code> = <code>total_deaths</code> + <code>total_killed_and_disposed_of</code>: "death"; If <code>total_cases</code> > <code>total_killed_and_disposed_of</code>: "death"; If <code>total_deaths</code> + <code>total_killed_and_disposed_of</code> > <code>total_cases</code>: "death"; If <code>total_cases</code> > <code>total_deaths</code>: "positive"; If <code>total_cases</code> > <code>total_killed_and_disposed_of</code>: "positive". 



#### Note

We have considered the two following values throughout the dataset: <br>

-   <code>NA</code> Not available: the information would be relevant for
    the event but the information was not mentioned in the WAHIS report. <br>  


## Contributors <a name="Contributors"></a>

- [Francesco Branda](https://francescobranda.netlify.app/) <br>

## Publications <a name="Publications"></a>
1) [Branda F, Giovanetti M, Scarpa F, Ciccozzi M. Monitoring avian influenza in mammals with real-time data. Pathogens and Global Health. 2024 Feb 29:1-5.](https://www.tandfonline.com/eprint/5NESRQXTYKYXTQGITT8G/full?target=10.1080/20477724.2024.2323843)


## License <a name="License"></a>

This project is licensed under the CC BY-SA 4.0 License - see the [CC
BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en) file
for details.

## Contact <a name="Contact"></a>

Francesco Branda. Email: 
[francesco.branda.contact@gmail.com](francesco.branda.contact@gmail.com)

## Disclaimer <a name="Disclaimer"></a>

*The World Organisation for Animal Health (WOAH) bears no responsibility
for the integrity or accuracy of the data contained herein, in
particular due, but not limited to, any deletion, manipulation, or
reformatting of data that may have occurred beyond its control.*
