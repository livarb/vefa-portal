+++

title = "Using EHF Catalogue tool"
group = "Generators"
type = "article"
draft = true

[[resources]]
title = "ERP systems that can help you send an EHF Catalogue"
url = "http://www.anskaffelser.no/verktoy/aksesspunkt-hvilke-kan-stotte-ditt-behov"

+++

Source: http://www.anskaffelser.no/verktoy/how-fill-ehf-catalogue-tool

Learn how to create your own catalogue XML file and send it through an access point.



If you would like to create an EHF file yourself, Difi has developed a catalogue template that can help you to generate an EHF catalogue in XML format. This file can either be used to send your electronic catalogue to your customer or be used by system developers to set up an automatic extract. This is built from address fields (catalogue headers) in order that the access point that will send the file to the buyer, knows where to send it. Under the main headers are fields in which one can fill out information on goods and services (catalogue lines).

## Step 1

Fill out the EHF Catalogue template header and line fields. Remember that a purchaser should be able to understand what they are ordering, so be precise with the information that you enter. See the explanation in the template or the video that is beside it.

The template itself contains codelists. For more detail on label and UNSPSC classification codes, see the links below.

* [Codes in EHF catalogue for labels](http://www.anskaffelser.no/verktoy/codes-use-ehf-catalogue-labels-environmental-and-social-responsibility)
* [Services and Tools - UNSPSC](http://www.anskaffelser.no/ehandelsplattformen/pages-english/services-and-tools-unspsc)

Click on the picture to see a larger version.

_Image: EHF Catalogue tool_

## Step 2

After filling out all the fields in the catalogue template, click on the symbol «Export to EHF format».

Choose a location to save the catalogue file to. Remember to mark it, so that you send the correct file.

EHF catalogue tool transformation keyEHF xml file

## Step 3

To make sure that that the file is correct, either you or your access point provider should validate the file before it is sent. This will ensure that the correct fields have been filled out.

When validating the file, it is important to use the notepad program on your computer, which removes any potential formatting that could create problems.

Click on the picture to see a larger version.

EHF Catalogue xml file open in notepad

In order to be sure that you have selected all the text, choose «Edit», then «Select all» and finally «Copy». 

Go to Difi’s validation tool at http://vefa.difi.no/formatvalidering/.

Paste in the code that you collected from your file. In the window underneath where you chose EHF catalogue, and click the «Validate XML» button.  As you can see in the image, if code is missing then two types of notifications are shown. If a mandatory filed is not filled out or filled out wrongly, a notification will appear that shows this (marked red).  As shown in the image, this is only a recommendation that it would be advisable to fill out the field in order to provide the buyer with information necessary for them to order correctly. 

If the file is correct, the validation too will notify you of this, at which point the file is ready to be sent to the buyer.

* [Contact an access point provider that can send the EHF Catalogue to your buyer](http://www.anskaffelser.no/verktoy/aksesspunkt-hvilke-kan-stotte-ditt-behov) (in Norwegian language only).

Ask the access point provider to explain where and how you should send or upload the file. 