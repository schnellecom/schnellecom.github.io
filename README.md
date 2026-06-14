# Lukas Schnelle's Personal Website

This repository contains the source code for my personal website: [https://lukasschnelle.de](https://lukasschnelle.de).

## Template Reference

This website is built using the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme, a simple, clean, and responsive theme for academics.

## Running Locally (Debian Environment)

To run this Jekyll website locally on a Debian-based environment, follow these steps:

1. **Install Ruby and required dependencies:**
   ```bash
   sudo apt-get update
   sudo apt-get install ruby-full build-essential zlib1g-dev imagemagick nodejs
   ```

2. **Set up your Ruby environment and install Bundler:**
   It is highly recommended to install gems in your user directory to avoid using `sudo`.
   ```bash
   echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
   echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
   echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   
   gem install jekyll bundler
   ```

3. **Install the project dependencies:**
   ```bash
   cd schnellecom.github.io
   bundle install
   ```

4. **Serve the website:**
   ```bash
   bundle exec jekyll serve --lsi
   ```
   The site will now be available at `http://127.0.0.1:4000/`.