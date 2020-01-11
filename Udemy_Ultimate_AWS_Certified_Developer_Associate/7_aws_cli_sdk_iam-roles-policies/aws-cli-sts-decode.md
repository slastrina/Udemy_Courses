# aws-cli-sts-decode

Found on exam

If an api call fails you get a long error message, this message can be decoded by the sts command line

Command: aws sts decode-authorization-message --encoded-message <message>

![example_sts](example_sts.png)

![sts_decoded_json](sts_decoded_json.png)

![sts-json-pretty-printed](sts-json-pretty-printed.png)