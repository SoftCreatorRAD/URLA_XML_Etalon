# URLA_XML_Etalon
URLA.XML v.3.4 with sample data according to iLAD

URLA XML file combines all possible XML fields with sample data, according to "MISMO iLAD industry Loan Application Dataset version 2.0.1 dated 05082020.xlsx".

The file will be used to test the XML data import:
1. Source: URLA XML
2. Target: set of SQL Server INSERT statements to import the data into a RDBMS.

To simplify the data validation, every field in the XML file has the value according to column AD (ULAD Form Field ID) in iLAD.
For example: Borrower Name (First)
Source XPath: MESSAGE/DEAL_SETS/DEAL_SET/DEALS/DEAL/PARTIES/PARTY/INDIVIDUAL/NAME
Source Attribute (DataPoint):  FirstName
ULAD Form Field ID (col AD) : 1a.1.1
Target DB Table: URLA Forms
DB Table Column: URLA_1a_1_1

The value in XML for this field should be: "URLA_1a_1_1"
