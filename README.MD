This is a small library written in PHP, which aims to send/retrieve data to/from the AdaFruit IO platform.

Example of use:

//wrapper to your AIO account

$aio = new AdaFruitIO(MY_ADAFRUIT_IO_PRIVATE_KEY);

//obtain a wrapper for the feed called "Test":

$feed = $aio->getFeed("Test");

$feed->send(1234); //sends "1234" to the feed called "Test"

echo $feed->get(); // echoes the last value sent to the feed, i.e. "1234"
