# google-speech-tts

A wrapper to google translate that generate a audio from a text.

```php
use GoogleSpeech\TextToSpeech;

$speech = new TextToSpeech();
$speech
    ->withLanguage('en-us')
    ->inPath('../audios');

for($i=0;$i<10;$i++){
    $speech->withName('output' . $i);
    $speech->download('new testing ' . $i);
}
```