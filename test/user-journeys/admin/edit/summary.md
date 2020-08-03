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
            <td style="border: 1px solid black; background-color: #218a5c;">
                Valid date (eg 27/03/2021)
            </td>
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
                <br>
                Month value greater than 12<br>
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