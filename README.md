# Academic Hosting 101 

A short guide about how to host your academic websites using [Jekyll](https://jekyllrb.com/).

## Creating simple, powerful websites and hosting them for free.

As an academic, its a common need to share information about your portfolio, or your class, or your next reading group. In this tutorial, we will use a very simple program, [Jekyll](https://jekyllrb.com/) to create such websites and host them free on Github using [Github Pages](https://pages.github.com/). Then, we will explore several off-the-shelf themes to make your website look good. Finally, we will cover one popular theme [al-folio](https://github.com/alshedivat/al-folio) using which you can share your portfolio as well as maintain a list of publications with your already exisiting bibtex.

## Installations

First, let us install the required tools in your system. 

### Install Jekyll

Jekyll is a Ruby Gem which can be [installed](https://jekyllrb.com/docs/installation/) in most systems. Ruby is a scripting language which powers the website builder toolkit Jekyll. Follow the instructions based on your system of choice:

#### Common installation - Linux or Mac

- Install Ruby Version Manager ([RVM](http://rvm.io/)). Open a Terminal (Control + Alt + T) and type the following commands:

([Check the instructions how to get gpg](https://usabilityetc.com/articles/ruby-on-mac-os-x-with-rvm/))

  ```
  gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
  ```
  and

  ```
  \curl -sSL https://get.rvm.io | bash -s stable --rails
  ```

- Install Ruby. Here we will use the version `2.3.1`

  ```
  rvm install 2.3.1
  ```

- Now that Ruby is installed, you can proceed to install Jekyll based on the system:

#### For Mac only

Copy paste the following in your Terminal:

-  Installs required dependencies to install Jekyll

  ```
  xcode-select --install
  ```

- Install the Jekyll Gem

  ```
  gem install --user-install bundler jekyll
  ```

- Open your bash config file. Its the file called `.bashrc` which is located in the home directory. You can edit the file using any editor of choice, here we will use `nano`. Type in the Terminal:

  ```
  nano ~/.bashrc
  ```

- This will open the file in your Terminal itself. Scroll down to the very end, and paste these two lines:

  ```
  export GEM_HOME=$HOME/gems
  export PATH=$HOME/gems/bin:$PATH
  ```

For more information / reference, [check this doc](https://jekyllrb.com/docs/installation/macos/).

#### For Ubuntu

- Make sure you have the required dependencies for Jekyll. Copy paste the following in your Terminal.

  ```
  sudo apt-get install build-essential zlib1g-dev
  ```

- Remember you already installed Ruby from the previous step. Now we just need to install the Jekyll Gem, which is the same procedure as for Mac:

  ```
  gem install jekyll bundler
  ```

Thats it! You can also [refer this document](https://jekyllrb.com/docs/installation/ubuntu/) for alternative ways to install.


#### Windows

- Install [RubyInstaller](https://rubyinstaller.org/downloads/), which will take care of the installation of Ruby. Download the top executable: `Ruby+Devkit 2.5.3-1 (x64)`. Run and install.

- Once installed, open a new command prompt, and type the following:

  ```
  gem install jekyll bundler
  ```

This should install Jekyll and necessary files.  If you need more information, refer to [this document](https://jekyllrb.com/docs/installation/windows/).

### Install Git

In order to use various templates off from the web to create your website, we would also need a popular version control system Git. You can get [all installation instructions here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Also, make sure you have created your [Github account](https://github.com/join) to be able to host your own webpages.

## Jekyll Theme Installation - Using al-folio theme

Jekyll provides a nice way to incorporate multiple themes for your website. In this tutorial, we will use the [al-folio](https://github.com/alshedivat/al-folio) theme which has a nice support for maintaining academic webpages including bibliography. To first install and run the theme, head over to the repository and "Fork" the repository to your own repository. You can give any name to your repository, ideally if you want Github to pick it up as your personal webpage then provide the name as `username.github.io`.

Then, open your Terminal / Command Prompt and run these commands as mentioned in the [installation guide](https://github.com/alshedivat/al-folio#installation):

```
$ git clone https://github.com/alshedivat/al-folio.git al-folio
$ cd al-folio
$ bundle install
$ bundle exec jekyll serve
```

Thats it! Let us first see how the default website looks like. Run the following from the folder in your terminal:

```
jekyll serve
```

This will open up the default website in your browser. If it didn't open up automatically, just head over to a browser and paste this in the run bar:

```
http://127.0.0.1:4000
```

## Building the website

Coming Soon
