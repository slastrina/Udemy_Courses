# Consistency_model

* "Read after write consistency" for PUTS of new objects
  * Can do a get immdiately after write for a new file
    * PUT 200 -> GET 200
  * This is true except if we did a get before to see if the object existed
    * GET 404 -> PUT 200 -> GET 404 eventually consistent
* "Eventually Consistent" for DELETES and PUTS of existing objects
  * if we read an object after updating we might get the older version
    * PUT 200 -> PUT 200 -> GET 200 (might be older version)
  * If we delete an object we might be a ble to retrieve it for a short time after
    * DELETE 200 -> GET 200


