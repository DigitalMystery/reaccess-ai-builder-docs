# ReAccess AI Introduction

The AI Documentation is meant to help both the user and AI to build out an Excel file which is used to create a new ReAccess app.  If you want to use the UI no-code solution please use our App Builder platform.  Below are the steps to create and excel doucment which you can then import in ReAccess.

## Steps

1.  Create an importable Excel document that ReAccess can consume.  

    To do this you must first create an Excel document normally with the Application Name as the document name.

2.  Create three tabs within the Excel document labeled Application, Forms, Controls

3.  On the Application tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Home" as the default.

    Application Tab Columns:

    A:  Name*

    B:  HomePageContent

    C   Tags*

    D:  Description*

    F:  Icon
    


4.  A form is synonymous to a page inside ReAccess.  It will house the data elements you wish to collect on which are called controls.  Here we will create the Form tab data elements.

  On the Forms tab the document must contain the following columns and make them bold if possible.  Anything with an asterisk is required from the user.  Also, tags are seperated by semicolons.  If an icon is not provided, use "Page" as the default.

    Form Tab Columns:

    A:  Name*
    B:  Scope*
    C   Tags*
    D:  Description*
    E:  ImportData
    F:  Icon*
    G:  Header
    H:  Footer
    I:  Integration Code
    J:  Sort Order*
    K:  Data Display Name
