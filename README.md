<p align="center">
  <img src="https://example.com/authextension.svg" alt="authextension" width="200" height="200" />
</p>

<h1 align="center">authextension</h1>

<h4 align="center">
  <a href="https://github.com/authextension">Repository</a> |
  <a href="https://docs.cloud">Documentation</a> |
  <a href="https://discord.cloud">Discord</a> |
  <a href="https://roadmap.cloud">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/authextension/actions"><img src="https://github.com/authextension/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/authextension"><img src="https://badge.fury.io/rb/authextension.svg" alt="Version"></a>
  <a href="https://github.com/authextension/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ API gateway for microservices 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install authextension
```

In your `Gemfile`:
```ruby
gem 'authextension'
```

### Run authextension

```bash
authextension --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/authextension.rb`:

```ruby
authextension::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = authextension::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'e2e_test.js' },
  { id: 2, title: 'roles' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [e2e_test.js] and [roles].

