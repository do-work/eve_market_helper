# EVE Industry Helper
EVE Online industry and market helper.

## Run
### Setup
1. Create new app at https://developers.eveonline.com/applications
1. Select the following scopes:
    1. esi-assets.read_assets.v1 
    1. esi-markets.read_character_orders.v1 
    1. esi-assets.read_corporation_assets.v1
1. Create `.env` file and populate with keys from `.env.example`
1. Add the provided `Client ID` and `Secret Key` values to your `.env` file.

### Turn on
`python app.py`

### SSO (one time only)
GET `/oauth/authorize`  
Authorize on CCP server the first time.  
Debug into the app to get the refresh token and save token to .`env` file.