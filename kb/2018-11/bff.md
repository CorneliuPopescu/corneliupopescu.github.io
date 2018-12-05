# Pattern: Backends For Frontends

> Rather than have a general-purpose API backend, instead you have one backend per user experience - or as (ex-SoundClouder) Phil Calçado called it a Backend For Frontend (BFF). Conceptually, you should think of the user-facing application as being two components - a client-side application living outside your perimeter, and a server-side component (the BFF) inside your perimeter.
>
> The BFF is tightly coupled to a specific user experience, and will typically be maintained by the same team as the user interface, thereby making it easier to define and adapt the API as the UI requires, while also simplifying process of lining up release of both the client and server components.

[Pattern: Backends For Frontends](https://samnewman.io/patterns/architectural/bff/){:target="_blank"} ![external redirect](../../img/ext-redir.png)

Tags: UI, API, Architecture

[_Back_](../)
