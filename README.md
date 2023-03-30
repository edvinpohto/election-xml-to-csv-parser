# election-xml-to-csv-parser
A two part Node.js script that takes in an XML file about Finnish elections and outputs a CSV file with information about candidate double mandates.

The script can easily be modified to take into account any other data that may be presented in the XML file.

The required XML files can be found on the [Tulospalvelu website](https://tulospalvelu.vaalit.fi/).
From there you can navigate to any of the listed elections, select Tulokset (results), and finally Ladattavat tiedostot (downloadable files) on the right hand side.
Presented with the download options, select Tulokset ehdokkaittain (results per candidate) under the XML-teidostot header.

Unzip the file (warning, it may be very large and often contains over a million lines of XML) and place in the same directory as your scripts.

Finally, make sure you set the filepath to your own XML file at the bottom of the main script file. Also create an "output" directory in the same location as your other files where the output CSV file will go.

Run <code>npm install</code> to install relevant dependencies.

Now you can run <code>node nodeXmlParser.js</code> to run the scripts.

Depending on the XML file size the execution may take a while.
