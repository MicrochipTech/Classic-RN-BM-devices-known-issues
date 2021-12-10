# Classic-RN-BM-devices-known-issues
This page captures all the known issues of classic RN BM devices.
<table>
  <tbody>
     <tr>
        <th>No.</th>
        <th>Device</th>
        <th>Type of Issue</th>
         <th> Issue</th>
        <th>Issue / Limitation</th>
        <th>Affected Version(s)</th>
        <th>Fix Version(s)</th>
        <th>Workaround</th>
    </tr>
    <tr>
          <td>1</td>
          <td> RN487x</td>
          <td>Firmware</td>
          <td>RN487x temperature sensor read failure</td>
          <td>  Background Details: Command @ reads one of the analog channels and returns the analog values in 16-bit hex format. Command @ expects one input parameter which is the analog channel in a single digit format. Analog part parameter 5 is related to Temperature sensor. 
@,5 reads the internal PTS temperature sensor data. 

Issue: Currently for V1.42 and prior firmware versions, the @,5 command response data is not accurate. This is due to the failure in ADC read. 

Solution: This issue will be get fixed by making a fix in the firmware. 
</td>
          <td> V1.42 and above</td>
          <td>Fix will be part of upcoming release. Release date not fixed</td>
          <td> No workaround available </td>
    </tr>
 </tbody>
</table>


