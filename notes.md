



https://chocolatey.org/install

@powershell -NoProfile -ExecutionPolicy Bypass -Command "[System.Net.WebRequest]::DefaultWebProxy.Credentials = [System.Net.CredentialCache]::DefaultCredentials; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH="%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

http://www.njtierney.com/jekyll/2015/11/11/how-i-built-my-site/
Step 1. Create a GitHub Account

Step 2. Create a github page, as per instructions here (https://pages.github.com/).
  > Repo name: <username>.github.io
  $ cd optixlab.github.io/
  $ git init
  $ git add --all # git add . also works?
  $ git commit -m "index file"
  $ git remote add origin git@github.com:optixlab/optixlab.github.io.git
  $ git push -u origin master

Step 3. Download requirements for jekyll (http://jekyllrb.com/docs/quickstart/)

Step 4. Follow directions from this blog (http://www.sitepoint.com/set-jekyll-blog-5-minutes-poole/)

Ruby on Windows:
	https://jekyllrb.com/docs/windows/
		$ choco install ruby -y
	https://labs.sverrirs.com/jekyll/1-ruby-and-devkit.html
		$ download devkit (http://rubyinstaller.org/downloads/)

	gem install jekyll bundler

	SSH errors
		http://guides.rubygems.org/ssl-certificate-update/#installing-using-update-packages
			2.6 available. Download this package
			c:\>gem install --local c:\rubygems-update-2.6.7.gem
			c:\>update_rubygems --no-ri --no-rdoc
			c:\>gem --version
			c:\>gem uninstall rubygems-update -x
			c:\>gem install jekyll bundler

Step 3.
	http://jekyllrb.com/docs/quickstart/

	$ cd ~/Dropbox/share/Projects/optixlab.github.io
	$ jekyll new . --force
