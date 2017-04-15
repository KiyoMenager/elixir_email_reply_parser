# ElixirEmailReplyParser

[![Build Status](https://travis-ci.org/hellogustav/elixir_email_reply_parser.svg?branch=master)](https://travis-ci.org/hellogustav/elixir_email_reply_parser)

Originally an Elixir port of https://github.com/github/email_reply_parser
as well as (especially) its port  of https://github.com/zapier/email-reply-parser

For retrieval of the last reply from email message text (body).

## Installation

The package can be installed by adding `elixir_email_reply_parser` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [{:elixir_email_reply_parser, "~> 0.1.0"}]
end
```

Published version of the docs can be found at [https://hexdocs.pm/elixir_email_reply_parser](https://hexdocs.pm/elixir_email_reply_parser).

## Usage

```elixir
    iex> email_content = "Hi!\n\n How are you?\n__________\nFrom: Some Author\n\n Previous email"
    iex> ElixirEmailReplyParser.parse_reply(email_content)
    "Hi!\n\n How are you?"
```
