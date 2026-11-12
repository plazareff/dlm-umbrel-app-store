# DLM Apps Umbrel Community Store

This is the community app store package for the `dlm-app-store` store ID.
Apps in this store must use IDs prefixed with `dlm-app-store-`.
The Tiiny Control Panel package includes its app icon.

## Install

1. Push this directory as the root of a public GitHub repository.
2. In umbrelOS, open **App Store → ⋯ → Community App Stores**.
3. Add the GitHub repository URL, open **DLM Apps**, and install Tiiny Control Panel.

The community package linter and local Docker smoke test pass. Installation
and Tiiny LAN connectivity still need validation on an actual umbrelOS device.
Community stores are independently maintained and aren't vetted by Umbrel.

## First launch

On the first launch, Tiiny Control Panel asks for a one-time setup code to give
your browser full access. In umbrelOS 2.x, open **Files**, find the Tiiny
Control Panel app-data folder, and open `setup-code.txt`. Copy the code into
the panel. Umbrel's Files app lets you browse app files; if you don't see this
file, make sure you are looking in the app's own data folder.

The full path is Applications->dlm-app-store-tiiny-control-panel->data->setup-code.txt

This is a one-time setup step: after the first browser is authorized, the setup
code is removed. Add any additional browsers or phones later from **System →
Devices** inside Tiiny Control Panel; they don't need the setup code again.

Keep the code private and only use it on a trusted device. It grants the first
browser full access to the panel. The code is stored in the app's persistent
data, so it remains available if you close the page before completing setup.
