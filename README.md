# Example for Solid Calendar Store blog post

This is the full example accompanying [our blog post](https://knows.idlab.ugent.be/blog/solid-calendar-store) 
about the [Solid Calendar Store](https://github.com/KNowledgeOnWebScale/solid-calendar-store/).

## Requirements

- Install dependencies via `npm i`.
- Download the latest RMLMapper jar from [here](https://github.com/RMLio/rmlmapper-java/releases).

## Usage

1. Start Community Solid Server via 

```shell
npm start
```

2. Request the busy calendar in JSON (default) via

```shell
curl http://localhost:3000/busy
```

3. Request the busy calendar in RDF (Turtle) via

```shell
curl -H 'accept: text/turtle' http://localhost:3000/busy
```

4. Request the busy calendar in ICS via

```shell
curl -H 'accept: text/calendar' http://localhost:3000/busy
```

## Configuration

The main configuration file is `config.json`.
It defines the different calendars and what operations are performed on them.
In the folder `config` we defined other configuration files, which contain,
for example, the converters and the routes used by the [Community Solid Server](https://github.com/solid/community-server).

## License
This code is copyrighted ©2019–2020 by [Ghent University – imec](http://idlab.ugent.be/)
and released under the [MIT license](http://opensource.org/licenses/MIT).
