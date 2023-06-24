
# Making thermal monitors yourself

We are working on instructions for making our thermal monitors.  Here are some pictures for the v3 monitor that will be sufficient for some solderers to assemble the hardware.  

```{image} /images/making/inside-of-battery-box.jpg
:alt: sensor unit
:class: bg-primary mb-1
:width: 400px
:align: center
```


```{image} /images/making/wiring-diagram.jpg
:alt: sensor unit
:class: bg-primary mb-1
:width: 400px
:align: center
```


```{image} /images/making/completed-build.jpg
:alt: sensor unit
:class: bg-primary mb-1
:width: 400px
:align: center
```

The build requires a battery box designed for 3AA batteries, with an on-off switch, an ESP12F microcontroller, a DHT22 temperature and relative humidity sensor, and cork.  

The ESP12F has to be flashed with the our software **before** it is soldered and this requires a matching burner board. The software will be open source but for now, contact us if you want to try this.

The order of soldering joins is not particularly important on this build.  The maker must cut the right size hole in the side of the battery box using a Stanley knife or similar, cut the cork to size, and glue parts in place.

Most of the battery consumption for our monitors is from keeping up a wifi connection.  This takes 100mA with spikes up to 200mA - 400mA. Each set of batch readings takes 4 seconds of wifi up time, and there are 14 batches sent a day. The v3 monitor batteries are 2200mAh, equating to around 20 hours of wifi service.  In theory that would mean more than a three year battery life, but we're really just hoping for a year.

We are experimenting with a build that use a single alkaline battery as this is might be more convenient for groups, but with the disadvantage of shorter battery life.   We are also experimenting with replacing the DHT22 with an HTU21 temperature and relative humidity sensor because we think this will give more accurate data and reduce the amount of wifi uptime required.

```{admonition} Important
If you intend to post devices to user groups, keep in mind that you need to comply with guidance about the packaging of batteries and that you may not ship used alkaline batteries by UK post.

- [IATA lithium battery guidance](https://www.iata.org/contentassets/05e6d8742b0047259bf3a700bc9d42b9/lithium-battery-guidance-document-2021.pdf) This is from the air industry but the rules are very widely adopted including by Royal Mail.
- [Royal Mail general battery guidance](https://www.postoffice.co.uk/mail/what-can-i-send)
```