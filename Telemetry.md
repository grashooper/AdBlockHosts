## TLDR

**AdAway do not record or send any personal data.**   
User can send crash and anonymous usage data if he/she want to.

## Telemetry

AdAway allows users to enable telemetry feature.
The telemetry feature provides two kinds of reports:
* Crash report and application failures,
* Application usage.
Both kinds of report does not contains any personal data.

Crash reports and application failures contains stacktrace (limited to current application context).
They are useful to find bugs and discover how much user are affected by.

Application usage contains information like which part of the application is used. For example, running tcpdump tool and malware analysis could be reported.
It is useful to understand what the user was doing when a bug happened.

Reports will include device information data like:
* Android device model,
* Android version,
* AdAway version.

Telemetry feature could freely be enabled and disabled at any time from application settings and will be applied immediately.

## Sentry

The telemetry feature is based on [Sentry](https://sentry.io/) platform and library.
Both are Open Source which comply with the AdAway vision of building an application you can trust (see [platform](https://github.com/getsentry/sentry) and [library](https://github.com/getsentry/sentry-java) GitHub projects).

As AdAway is Free and Open Source software, we don't have money to run own instance of telemetry platform. So sentry.io is used to gather application reports.

If you want to learn more about Sentry, check [the Mozilla detailed documentation](https://github.com/mozilla-mobile/focus-android/wiki/Crash-Reporting-with-Sentry) which use Sentry for crash reporting on Firefox Focus.

## FAQ

* _Why include telemetry in AdAWay?_

Telemetry should help a lot to improve the application. Only few users report bug and attach logcat on GitHub issues or development forum. It offers a way to anyone to contribute to the application development.

* _But I don't want telemetry!_

The telemetry feature is disabled by default. It will only work if you consent to and enable it.

* _But I don't want any telemetry library shipped or running into my device!_

The application source code comes with a `sentrystub` module. It could replace the Sentry library at build time in order to compile. A such variant is the default behavior on development builds distributed on development forum.