# Dev Log

## 2020-06-30

* Rough implementation on v0.10.0-alpha1
* Setup environment for admin user (pgpass, pg_service, env vars,)
* Application install script will have environ
* Fix nofile limit on postgres|pgbouncer|patroni
* [Milestone](./milestone.md) planning.


## 2020-06-29

* Remake release system
* Have a draft on application installation standard
* Use 'v' prefixed fully qualified version string
* remove polysh from default pkg (unstable when downloading) 
* remove grafana plugins, since lot's of them were covered in grafana 8.0


## 2020-06-28

* Remake alerting rules 


## 2020-06-25

* Remake infra-rules and pgsql-rules

## 2020-06-23

* Remake PGSQL node


## 2020-06-10

It's time to have an overhaul on monitoring system, which includes:
* Upgrade `pg_exporter` to 0.4.0 , re-write metric definition and add support for PostgreSQL 14  
* Use static file service discovery by default to reduce dependency for monitoring system
* Use static label set (job,cls,ins), remove (svc,role,ip) from labels, Which makes identity immutable
* Redesign entire monitoring system to use new label system and embrace Grafana 8.0
* Using grafana 8.0 new features

## 2020-06-01

Well it's good to write some dev logs.