# Security

This section contains information on Security Standards for services.

# Security hardware and software

## Proxies

* PCI proxies
    - Is this the way we wan to do things going forward?
    - In what other ways would we use proxies?
* Nginx use for forwarding for external customers.
* DMZ Zone
* Defense in depth

## Gateways

* What do we mean by gateways?
* What would we use them for?

## Firewalls

* We currently use physical firewalls.
* Where would we use software firewalls?
    - What does that gain us?

# Authentication

1.  Services must authenticate all calls by validating the X-Auth-Token HTTP Header against the internal or external Global Auth / Identity services
    1.  Optional support for BullFrog as required
2.  No service accounts or shared username / passwords
    - Do we need to call Identity for internal services?
    - No service accounts? What do we currently do?

# Authorization

1.  Services must use either Global Auth/Identity Roles or (usually) LDAP permissions to authorize role based actions
    - Reuse
    - Rate-limiting
    - RBAC
    - Consistency

# SSL

1.  All Services must use SSL for API end-points

# Code Review/Vulnerability Scanning

1.  All services should participate in a code review by the GSS team prior to each major release.
2.  Services should execute vulnerability scanning as part of the continuous integration build for their service.
3. Vulnerability assessment
4. Products Security (Security Engineering)
5. Code Review
6. API Review
7. Threat modeling

## GSS

* PCI - Vulnerability assessment
* Hardening script - scans entire network - [CIS_CAT](http://benchmarks.cisecurity.org/downloads/audit-tools/#cis-cat)

## Action Items:

* Ask identity about disabling a user and token
