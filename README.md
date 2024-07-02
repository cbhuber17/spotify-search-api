## Install

```sh
cargo build
```

## Usage

```sh
cargo run "[search query]" "[Spotify auth token]"
```

You'll need an authentication token to make search queries! Log into your spotify account on a web browser.

Create a `.env` file with the following inside of it:

```
CLIENT_ID=<CLIENTID>
CLIENT_SECRET=<CLIENTSECRET>
```

Where `CLIENT_ID` and `CLIENT_SECRET` come from your settings when creating a new developer project at https://developer.spotify.com/.

Next, with python 3.12, perform the following:

```
python -m venv token_env
```

Active the new virtual environment as follows:

```
cd token_env
cd Scripts
activate
cd..
cd..
```

(token_env should appear in the CLI).

Then install the required dependencies:

```
pip install -r requirements.txt
```

Run the python script to capture the token:

```
python get_token.py
```

The token will be printed to the screen and placed in `token.txt`.
