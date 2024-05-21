<p align="center">
  <picture>
    <source srcset="https://github.com/karimawi/TE-QuotaCheck/assets/69881381/38fc894a-9608-49eb-b8a4-6106e6845d46" media="(prefers-color-scheme: dark)">
    <img src="https://github.com/karimawi/TE-QuotaCheck/assets/69881381/c03d3254-bf0c-4aaf-bdde-0f27b94c7549" alt="(WE) Telecom Egypt Quota Check" height="150px"">
  </picture>
</p>
<br>

<p>
A Program written in Python that fetches your current quota details for WE (Telecom Egypt) ISP subscribers using their updated API, without you having to log in every time, this can be used and implemented in several ways, like regularly fetching and saving the results to calculate or graph usage, monitor consumption for SMEs who rely on an internet connection for their activities to calculate costs, and many other applications that may not be possible with just the mobile app or the website wich are not that quick when you have to login every single time.

  <br>
  
<h6>⚠️Please note that this program is not officially or directly affiliated with Telecom Egypt. The use of their API is conducted independently and is not based on any contractual agreement or formal association with Telecom Egypt. Additionally, Telecom Egypt holds the copyrights to the original branding, which has been used and slightly modified in this README.<h6/>
<p/>
<br>
  
### Preview:

![image](https://github.com/karimawi/TE-QuotaCheck/assets/69881381/e3cf28fb-4292-4f23-a425-b4ee034c41d4)


### Information Pulled:
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

### Configuration
Follow at lines 9-11 (lol) in the [main.py](./main.py#L9) file
```py
# Your credentials
lnd_number = "YOUR_LANDLINE_NUMBER" # Example: 0234567891 (make sure to have the 02 at the beginning
lnd_pass = "YOUR_PASSWORD" # If you don't know or remember your password, you can reset it by clicking "Forgot Password?" at my.te.eg
```

### License
You can use this however you want, but consider mentioning this Repo if you're going to use my code in an open-source project as I spent quite some time reverse-engineering their API after they had changed the authentication method.
