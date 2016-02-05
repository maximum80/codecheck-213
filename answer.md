Hi All,

I implemented it using Play 2.4.2 and Slick 3.0, with Scala. I also added a couple of open-source plugins for working with Redis as well as a driver for Joda Dates support for Slick.

I tried to learn Play, Slick, and Scala as I went along (I have some functional programming experience thanks to some Lisp/Scheme exposure and working with Javascript and Coffeescript, so those helped) to make this project over the past 4 days, so there are parts of my code that aren't as succinct and concise as I would have hoped.All the tests pass though.

I also encountered some trouble with provisioning (for some reason, `{{os_user_name}}` is null, breaking the mysql installation), but I tried to fix my Vagrantfile and Ansible provisioning scripts and make them as stable as possible. I hope you don't encounter any trouble setting up my environment.

After running `vagrant up`, do the following:
```bash
vagrant provision
vagrant ssh
mysql -uvagrant -pvagrant -Dvagrant < scala-test/sql/create.sql
cd scala-test
npm install
cd ticket-serv
activator
```

I also added these instructions to the modified README.

Thanks!
