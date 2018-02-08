**`TA-get-me`**

Get web API data into Splunk

This Splunk app is a pure fun app and was used in my Darksky Photographie Splunk app at .conf 2017 talk:

**Take a talk into the art of dark sky photography with a splunk ninja**

[https://conf.splunk.com/files/2017/slides/take-a-talk-into-the-art-of-dark-sky-photography-with-a-splunk-ninja.pdf]()

**Install:**

Install as usual in the Splunk web or copy into $SPLUNK_HOME/etc/apps (don't use it on a prod system!)

**Configure:**

Copy 'default/inputs.conf' to 'local/'

**Moon API** - nothing to do here, move along.

**Weather API** - get your API key from http://api.openweathermap.org and use the Splunk web to configure the input.

**Google directions** - get your API key from https://developers.google.com/maps/documentation/directions/get-api-key and use the Splunk web to configure the input.

**Usage:**

Use the custom search command `get` to either get:

    moon data ( | get me=moon )
    Weather ( | get me=weather ... )
    Google directions ( | get me=directions ... )
    or to get the easter egg ;)

**Debug**

Debug option can be enabled in the Splunk Web using the settings in the data input,
and change the debug option in the `debug setting` stanza from `no` to `yes`.

**Support**

This is an open source project, no support provided, but you can ask questions
on answers.splunk.com and I will most likely answer it.
Github repository: https://github.com/M-u-S/TA-get-me
