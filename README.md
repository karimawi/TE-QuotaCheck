<p align="center">
  <picture>
    <source srcset="https://i.imgur.com/mV5Q1bL.png" media="(prefers-color-scheme: dark)">
    <img src="https://i.imgur.com/31oBfHU.png" alt="(WE) Telecom Egypt Quota Check" height="150px"">
  </picture>
</p>
<br>

<p>
A Program written in Python that fetches your current quota details for WE (Telecom Egypt) ISP subscribers using their updated API, without you having to log in every time, this can be used and implemented in several ways, like regularly fetching and saving the results to calculate or graph usage, monitor consumption for SMEs who rely on an internet connection for their activities to calculate costs.
<p/>
<be>
  
### Preview:

![image](https://github.com/karimawi/TE-QuotaCheck/assets/69881381/e3cf28fb-4292-4f23-a425-b4ee034c41d4)


### Information Displayed:
<p>
<ul>
  <li>Landline Owner Name</li>
  <li>Offer Name</li>
  <li>Total GBs</li>
  <li>Used GBs</li>
  <li>Reminaing GBs</li>
  <li>Date and Time of Last Renewal (UNIX Timestamp later converted to readable date and time)</li>
  <li>Date and Time of Next Renewal (UNIX Timestamp later converted to readable date and time)</li>
</ul>
<p/>

### Other Calculated Information:
<p>
<ul>
  <li>Usage Percentage</li>
  <li>Days or Hours (if less than a day) until expiration</li>
</ul>
<p/>

### Requirements
Basically, everything is PSL (Python Standard Library) except for [Requests](https://github.com/psf/requests) which I'm using version 2.31.0 of
```ps
pip install requests==2.31.0
```

### License
You can use this however you want, but consider mentioning this Repo if you're going to use my code in an open-source project as I spent quite some time reverse-engineering their API after they had changed the authentication method.
