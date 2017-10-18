# Twilex

Twilex is an Elixir Client to send SMS/MMS using Twilio.

## Install

Add twilex to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [{:twilex, git: "https://github.com/Waasi/twilex"}]
end
```

## Configure

Add the following to your `config.exs` file:

```elixir
config :twilex,
  sid: "YOUR_TWILIO_SID",
  token: "YOUR_TWILIO_AUTH_TOKEN"
```

## Usage

```elixir
 # Twilex.Messenger.send_sms("from_number", "to_number", "body_text", "optional_media_url")
 iex(1)> Twilex.Messenger.send_sms("15005550006", "15005550001", "test text", "https://github.com")
```

## Author

The author of this library is Yinghai Zhao (@hisea).
