---
slug: basic-auth-login
title: HTTP basic authentication login
sidebar_label: HTTP basic auth
sidebar_position: 8
description: a resource protected by HTTP basic authentication, prompting for credentials through the browser's native dialog
---

The linked resource responds with `401 Unauthorized` and a `WWW-Authenticate: Basic` challenge, so the browser collects the username and password in its own credential dialog rather than in page markup. Any non-empty username and password are accepted.

Credentials are cached by the browser for the protection space, so a new dialog will only appear after the cache is cleared (typically by restarting the browser or opening the resource in a private window).

<div class="container margin-vert--xl">
  <div class="row">
    <div class="card col col--12 padding--md">
      <div class="card__body">
        <a class="button button--primary" href="pathname:///basic-auth">Login</a>
      </div>
    </div>
  </div>
</div>
<hr/>
