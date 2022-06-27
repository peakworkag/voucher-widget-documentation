# Peakwork Voucher Web Component (PREVIEW)
## About
This repository shows how the Peakwork web component can be embedded into any website.

To get an api key reach out to your Peakwork Contact. 
You will have to specifify domain names (and ports) for which the api key will be valid.

## Events
The widget/web component exports the following events.
The Payload is always retrieved via ```event.details```.

| Event Name |Payload| 
|------------|---|
|voucher-creation-started|```{message: string}```|
|voucher-created|```{message: string}```|
|voucher-creation-failed|```{message: string; errorCode: string;}```|
|template-load-failed|```{message: string; errorCode: string;}```|


We recommend implementing some sort of feedback loop for the customer based on the events, 
e.g. starting a spinner on creation started and success/error messages on creation/creation failed.