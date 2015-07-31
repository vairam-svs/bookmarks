https://github.com/IdentityServer/IdentityServer3.MembershipReboot

Source: https://github.com/IdentityServer/IdentityServer3.MembershipReboot
Nuget: http://www.nuget.org/packages/BrockAllen.MembershipReboot/
http://brockallen.com/2013/07/29/announcing-membershipreboot/: 
MembershipReboot is a user identity management and authentication library. It has nothing to do with the ASP.NET Membership Provider, but was inspired by it due to frustrations with the built-in ASP.NET Membership system. The goals are to improve upon and provide missing features from ASP.NET Membership. It is designed to encapsulate the important security logic while leaving most of the other aspects of account management either configurable or extensible for application developers to customize as needed.

Some of the features of MembershipReboot are:

single- or multi-tenant account management
flexible account storage design (relational/SQL or object/NoSql)
claims-aware user identities
support for account registration, email verification, password reset, etc.
account lockout for multiple failed login attempts (password guessing)
extensible templating for email notifications
customizable username, password and email validation
notification system for account activity and updates (e.g. for auditing)
account linking with external identity providers (enterprise or social)
proper password storage (via PBKDF2)
configurable iterations
defaults to OWASP recommendations for iterations (e.g. 64K in year 2012)
Two factor authentication support via mobile phone SMS messages
The most common use case will be to integrate this into an ASP.NET or ASP.NET MVC application, though the library can also be used over a network as a service.

