<table style="border: 1px solid black;">
  <thead>
    <tr>
      <th colspan="5" style="border: 1px solid black;">Create an exercise "exercises/new"</th>
    </tr>
  </thead>
  <tbody style="border: 1px solid black;">
    <tr style="border: 1px solid black;">
      <td style="border: 1px solid black;">Item/Field</td>
      <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">Positive Testing</td>
      <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">Negative Testing</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Exercise name</td>
      <td style="border: 1px solid black; background-color: #218a5c;">String value (eg. Test exercise)</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;" >
      1 char value<br>
      1 num value<br>
      1 special character value<br>
      No value<br>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">"Add more information" Radio</td>
      <td style="border: 1px solid black; background-color: #218a5c;">"Yes"<br>"No - I'll do this later"<br></td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;" >
      No value selected<br>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">"What do you want to add?" Checkbox (Yes selected above)</td>
      <td style="border: 1px solid black; background-color: #218a5c;">
      Select all<br>
      Select one<br>
      ...etc<br>
      Any combination of boxes checked<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;" >
      None selected<br>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr>
      <td style="border: 1px solid black;">Save and continue Button</td>
      <td style="border: 1px solid black; background-color: #218a5c;">
      Click when all fields are filled<br>
      Click when not all fields are filled<br>
      Click when no fields are filled</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">Double click<br>spam click<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
  </tbody>
</table>

Rest of document assumes all options for adding info have been checked

<table style="border: 1px solid black;">
  <thead>
    <tr>
      <th colspan="5" style="border: 1px solid black;">Website listing "exercises/:id/edit/summary"</th>
    </tr>
  </thead>
  <tbody style="border: 1px solid black;">
    <tr style="border: 1px solid black;">
      <td style="border: 1px solid black;">Item/Field</td>
      <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">Positive Testing</td>
      <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">Negative Testing</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Exercise name</td>
      <td style="border: 1px solid black; background-color: #218a5c;">String value (eg. Test exercise)</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;" >
      1 char value<br>
      1 num value<br>
      1 special character value<br>
      No value<br>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Estimated launch date</td>
      <td style="border: 1px solid black; background-color: #218a5c;">Valid Date (eg 03/2021)</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">
      Empty value<br>
      <br>
      Only month val<br>
      Only year val<br>
      <br>
      <br>
      Year in past (eg. 01/2019)<br>
      Month in past (eg. 01/2020)<br>
      Year over 10(?) years in future (eg. 01/2030)<br>
      <br>
      Month value greater than 12<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Add launch day button</td>
      <td style="border: 1px solid black; background-color: #218a5c;">Click</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">
      double click<br>
      spam click<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Estimated launch date With launch day</td>
      <td style="border: 1px solid black; background-color: #218a5c;">Valid date (eg 27/03/2021)</td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">
      Empty value<br>
      <br>
      Only day val<br>
      Only month val<br>
      Only year val<br>
      <br>
      Only day + month val<br>
      Only day + year val<br>
      Only month + year val<br>
      <br>
      Year in past (eg. 01/01/2019)<br>
      Year over 10(?) years in future (eg. 01/01/2031)<br>
      <br>
      Day value greater than ammount of days in month [Leap years considered] (eg. "32/01/1980" or "30/02/1980" or "31/04/1980")<br>
      <br>Month value greater than 12
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Role summary<br>
      <strong>[Assuming a limit of 1000 chars]</strong><br>
      </td>
      <td style="border: 1px solid black; background-color: #218a5c;">
        1000 chars<br>
        1000 chars inc numbers<br>
        1000 chars inc special chars<br>
        1000 chars inc numbers and special chars<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">
        Empty value<br>
        Only numbers<br>
        Only special characters<br>
        Only numbers and special characters<br>
        1001 chars<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
    <tr >
      <td style="border: 1px solid black;">Subscriber alerts url</td>
      <td style="border: 1px solid black; background-color: #218a5c;">
        Valid URL<br>
        No value<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
      <td style="border: 1px solid black; background-color: #8a2621;">
        Non-existant domain<br>
      </td>
      <td style="border: 1px solid black;">[ ]</td>
    </tr>
  </tbody>
</table>
<br>
<table style="border: 1px solid black;">
    <thead>
        <tr>
            <th colspan="5" style="border: 1px solid black;">Contacts "exercises/:id/edit/contacts"</th>
        </tr>
    </thead>
    <tbody style="border: 1px solid black;">
        <tr style="border: 1px solid black;">
            <td style="border: 1px solid black;">Item/Field</td>
            <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">Positive Testing</td>
            <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">Negative Testing</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Exercise mailbox</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            String value (eg. Test exercise)<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
                invalid Email Address value<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Email signature name
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid name string
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                1 character value<br>
                1 number value<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Exercise phone number
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                    Valid UK mobile number (eg. +44 7911 123456)<br>
                    Valid UK mobile number, no country code (eg. 07911 123456)<br>
                    Valid UK landline number(eg. +44 1234 567890)<br>
                    Valid UK landline number, no country code (eg. 01234 567890)<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                No value<br>
                100 number value<br>
                9 number value<br>
                11 character string value<br>
                11 special character string value<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Senior selection exercise manager
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection exercise manager
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection exercise officer
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid "***.judicialappointments.digital" Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                Valid Email address<br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Assigned commissioner
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Other contacts - Appropriate authority
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Select one<br>
                Select two<br>
                ...<br>
                Select all apart from other<br>
                Select other - give valid string<br>
                Select all including other - give valid string<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
                Select other - give no string<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                HMCTS or Welsh Government lead contact
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                HMCTS or Welsh Government contact
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Judicial Office contact
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Lead judge</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Drafting judge</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Statutory Consultee</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Email address 
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value <br>
                No @ symbol<br>
                Non-existant domain<br>
                100 characters name<br>
                Special characters<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">'Add another' button</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Single click<br>
            5 x click<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
            ?<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">'Remove' button</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Single click<br>
            5 x click<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
            ?<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">Save and continue Button</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Click when all fields are filled<br>
            Click when not all fields are filled<br>
            Click when no fields are filled</td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">Double click<br>spam click<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
    </tbody>
</table>
<br>
<table style="border: 1px solid black;">
  <thead>
    <tr>
      <th colspan="5" style="border: 1px solid black;">Shortlisting methods “exercises/:id/edit/shortlisting”</th>
    </tr>
  </thead>
    <tbody style="border: 1px solid black;">
        <tr style="border: 1px solid black;">
            <td style="border: 1px solid black;">Item/Field</td>
            <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">Positive Testing</td>
            <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">Negative Testing</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Shortlisting methods
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Select "Situational judgement qualifying test (QT)"<br>
                Select "Critical analysis qualifying test (QT)"<br>
                Select "Scenario test qualifying test (QT)"<br>
                Select "Name blind paper sift"<br>
                Select "Paper sift"<br>
                Select "Telephone assessment"<br>
                Select all apart from other<br>
                Select other - give valid string<br>
                Select all including other - give valid string<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
                Select other - give no string<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Other - Add another
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Select other - add another - give both valid strings<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;" >
                Select other - add another - give no string<br>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">Save and continue Button</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Click when all fields are filled<br>
            Click when not all fields are filled<br>
            Click when no fields are filled</td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">Double click<br>spam click<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
    </tbody>
</table>
<br>
<table style="border: 1px solid black;">
    <thead>
        <tr>
            <th colspan="5" style="border: 1px solid black;">
                Timeline “exercises/:id/edit/timeline”
            </th>
        </tr>
    </thead>
    <tbody style="border: 1px solid black;">
        <tr style="border: 1px solid black;">
            <td style="border: 1px solid black;">Item/Field</td>
            <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">Positive Testing</td>
            <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">Negative Testing</td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">Open for applications</td>
            <td style="border: 1px solid black; background-color: #218a5c;">Valid Date in future (eg. 01/10/2020)</td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only day val<br>
                Only month val<br>
                Only year val<br>
                <br>
                Only day + month val<br>
                Only day + year val<br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/01/2019)<br>
                Year over 10(?) years in the future (eg. 01/01/2031)<br>
                <br>
                Day value greater than ammount of days in month [Leap years considered] (eg. "32/01/2024" or "30/02/2024" or "31/04/2024")
                <br>
                Month value greater than 12<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            </tr>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Closed for applications</td>
            <td style="border: 1px solid black; background-color: #218a5c;">Valid Date further in future than open date (eg. 01/10/2020)</td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only day val<br>
                Only month val<br>
                Only year val<br>
                <br>
                Only day + month val<br>
                Only day + year val<br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/01/2019)<br>
                Year over 10(?) years in the future (eg. 01/01/2031)<br>
                <br>
                Day value greater than ammount of days in month [Leap years considered] (eg. "32/01/2024" or "30/02/2024" or "31/04/2024")
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Shortlisting - Shortlisting Outcome</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020) <br>
            (??? and after closed for applications date ???)
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">Independent Assessors - Contact Independent assessors</td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020)
            (??? and after closed for applications date ???)
            (??? and after closed for shortlisting outcome date ???)
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
            Independent Assessors - Independent Assessments return date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020) and after contact independent assessors date <br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???)
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
            Independent Assessors - Independent Assessments hard limit
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020) and after contact independent assessors date <br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???)
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Eligibility SCC - Eligibility SCC date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020) <br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???) <br>
            (???) and after contact independent assessors date <br>
            (??? and after closed for IA return/hard limit date ???) <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Selection Day - Selection day start
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020)<br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???) <br>
            (???) and after contact independent assessors date <br>
            (??? and after closed for IA return/hard limit date ???) <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to Contact Independent assessors date<br>
                (???) Date prior to Contact Independent assessments return date<br>
                (???) Date prior to Contact Independent assessments hard limit<br>
                (???) Date prior to shortlisting outcome date<br>
                (???) Date after selection day end <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day end
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020)<br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???) <br>
            (???) and after contact independent assessors date <br>
            (??? and after closed for IA return/hard limit date ???) <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to Contact Independent assessors date<br>
                (???) Date prior to Contact Independent assessments return date<br>
                (???) Date prior to Contact Independent assessments hard limit<br>
                (???) Date prior to shortlisting outcome date<br>
                (???) Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        <tr >
            <td style="border: 1px solid black;">
                Selection Day - Selection day start
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020)<br>
            (??? and after closed for applications date ???) <br>
            (??? and after closed for shortlisting outcome date ???) <br>
            (???) and after contact independent assessors date <br>
            (??? and after closed for IA return/hard limit date ???) <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to Contact Independent assessors date<br>
                (???) Date prior to Contact Independent assessments return date<br>
                (???) Date prior to Contact Independent assessments hard limit<br>
                (???) Date prior to shortlisting outcome date<br>
                (???) Date after selection day end <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day end
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                (??? and after closed for applications date ???) <br>
                (??? and after closed for shortlisting outcome date ???) <br>
                (???) and after contact independent assessors date <br>
                (??? and after closed for IA return/hard limit date ???) <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                <br>
                Only month val<br>
                Only year val<br>
                <br>
                Only month + year val<br>
                <br>
                Year in past (eg. 01/2019)<br>
                Year over 10(?) years in the future (eg. 01/2031)<br>
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                (???) Date prior to closed for applications date<br>
                (???) Date prior to Contact Independent assessors date<br>
                (???) Date prior to Contact Independent assessments return date<br>
                (???) Date prior to Contact Independent assessments hard limit<br>
                (???) Date prior to shortlisting outcome date<br>
                (???) Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
        </tr>
            <td style="border: 1px solid black;">
                Selection Day - Location
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid string<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                Only numbers<br>
                Only special chars<br>
            </td>
            <td style="border: 1px solid black;">[ ]</td>
        </tr>
    </tbody>
  </table>
