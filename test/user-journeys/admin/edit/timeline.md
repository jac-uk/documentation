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
            <td style="border: 1px solid black;">
                Item/Field
            </td>
            <td colspan="2" style="border: 1px solid black; background-color: #218a5c;">
                Positive Testing
            </td>
            <td colspan="2" style="border: 1px solid black; background-color: #8a2621;">
                Negative Testing
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Open for applications
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date in future (eg. 01/10/2020)
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
            <td style="border: 1px solid black;">
                [ ]
            </td>
            </tr>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Closed for applications
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Shortlisting - Shortlisting Outcome
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
            Valid Date further in future than open date (eg. 01/10/2020) <br>
            and after closed for applications date
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Date prior to closed for applications date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Independent Assessors - Contact Independent assessors
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)
                and after closed for applications date
                and after closed for shortlisting outcome date
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to closed for applications date<br>
                Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Independent Assessors - Independent Assessments return date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020) and after contact independent assessors date <br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to closed for applications date<br>
                Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Independent Assessors - Independent Assessments hard limit
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020) and after contact independent assessors date <br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to closed for applications date<br>
                Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Eligibility SCC - Eligibility SCC date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020) <br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to closed for applications date<br>
                Date prior to shortlisting outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day start
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date after selection day end <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day end
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day start
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date after selection day end <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection Day - Selection day end
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020) and after selection day start <br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Selection Day - Location
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid string<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Empty value<br>
                Only numbers<br>
                Only special chars<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Character Checks - Character Checks request date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date <br>
                and after closed for IA return/hard limit date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                after character checks return date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Character Checks - Character Checks return date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start <br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Statutory Consultation - Statutory Consultation date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Character and Selection SCC - Character and SCC date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Final Outcome - Final outcome to candidates
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Equal merit dates - Second stage start date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
                and after Final outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
                Date prior to Final outcome date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Equal merit dates - Second stage end date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
                and after Final outcome date<br>
                and after Second stage start date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
                Date prior to Final outcome date<br>
                Date prior to Second stage start date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Equal merit dates - Second stage end date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
                and after Final outcome date<br>
                and after Second stage start date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
                Date prior to Final outcome date<br>
                Date prior to Second stage start date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Equal merit dates - EMP SCC date
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
                and after Final outcome date<br>
                and after Second stage start/end date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                <br>
                Month value greater than 12<br>
                <br>
                Date prior to open for applications date<br>
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
                Date prior to Final outcome date<br>
                Date prior to Second stage start/end date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Equal merit dates - EMP Outcomes
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid Date further in future than open date (eg. 01/10/2020)<br>
                and after closed for applications date<br>
                and after closed for shortlisting outcome date<br>
                and after contact independent assessors date<br>
                and after closed for IA return/hard limit date<br>
                and after Character Checks request/return dates<br>
                and after Statutory consultation date<br>
                and after Character and SCC date<br>
                and after Final outcome date<br>
                and after Second stage start/end date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
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
                Date prior to character checks request date <br>
                Date prior to closed for applications date<br>
                Date prior to Contact Independent assessors date<br>
                Date prior to Contact Independent assessments return date<br>
                Date prior to Contact Independent assessments hard limit<br>
                Date prior to shortlisting outcome date<br>
                Date prior to selection day start<br>
                Date prior to Character Checks request/return dates<br>
                Date prior to Statutory consultation date<br>
                Date prior to Character and SCC date<br>
                Date prior to Final outcome date<br>
                Date prior to Second stage start/end date<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
        <tr>
            <td style="border: 1px solid black;">
                Continue Button
            </td>
            <td style="border: 1px solid black; background-color: #218a5c;">
                Click when all fields are filled<br>
                Click when not all fields are filled<br>
                Click when no fields are filled<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
            <td style="border: 1px solid black; background-color: #8a2621;">
                Double click<br>
                spam click<br>
            </td>
            <td style="border: 1px solid black;">
                [ ]
            </td>
        </tr>
    </tbody>
</table>