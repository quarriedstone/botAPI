# botAPI
REST API for CatBreadBot communication written using Flask and Telethon

# Documentation
### **/register/register**: 

Register by sending /register/register with two parameters `user_id` and `phone`. After you get code via SMS, proceed to /register/register with parameter `user_id`, `phone` and `code`. After that you may use this API. 

### **/register/check**:

If you want to check the registration use /register/check with parameter `user_id`.

### **/sendMessage**:

Send message to bot by sending /sendMessage with `user_id`

### **/getMessages**:

Get last messages from bot conversation. Get message by sending /getMessage with `user_id`. You may also specify number of messages to get by specifying `limit`. If `limit` is not specified, last message is returned

# Future enhancements
1) Make registration as another service. 

2) Provide token from external service. Make API as /token/<command>.

3) Add Settings file.

4) Add external database support.

5) Make all API calls uniform, by returning JSON files in each call.
