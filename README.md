[![npm](https://img.shields.io/npm/v/kronos-service-koa.svg)](https://www.npmjs.com/package/kronos-service-koa)
[![Greenkeeper](https://badges.greenkeeper.io/Kronos-Integration/kronos-service-koa.svg)](https://greenkeeper.io/)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/Kronos-Integration/kronos-service-koa)
[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Build Status](https://secure.travis-ci.org/Kronos-Integration/kronos-service-koa.png)](http://travis-ci.org/Kronos-Integration/kronos-service-koa)
[![codecov.io](http://codecov.io/github/Kronos-Integration/kronos-service-koa/coverage.svg?branch=master)](http://codecov.io/github/Kronos-Integration/kronos-service-koa?branch=master)
[![Coverage Status](https://coveralls.io/repos/Kronos-Integration/kronos-service-koa/badge.svg)](https://coveralls.io/r/Kronos-Integration/kronos-service-koa)
[![Known Vulnerabilities](https://snyk.io/test/github/Kronos-Integration/kronos-service-koa/badge.svg)](https://snyk.io/test/github/Kronos-Integration/kronos-service-koa)
[![GitHub Issues](https://img.shields.io/github/issues/Kronos-Integration/kronos-service-koa.svg?style=flat-square)](https://github.com/Kronos-Integration/kronos-service-koa/issues)
[![Dependency Status](https://david-dm.org/Kronos-Integration/kronos-service-koa.svg)](https://david-dm.org/Kronos-Integration/kronos-service-koa)
[![devDependency Status](https://david-dm.org/Kronos-Integration/kronos-service-koa/dev-status.svg)](https://david-dm.org/Kronos-Integration/kronos-service-koa#info=devDependencies)
[![docs](http://inch-ci.org/github/Kronos-Integration/kronos-service-koa.svg?branch=master)](http://inch-ci.org/github/Kronos-Integration/kronos-service-koa)
[![downloads](http://img.shields.io/npm/dm/kronos-service-koa.svg?style=flat-square)](https://npmjs.org/package/kronos-service-koa)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

# kronos-service-koa

koa backed http server

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [ServiceKOA](#servicekoa)
    -   [Parameters](#parameters)
    -   [Properties](#properties)
    -   [name](#name)
-   [RouteSendEndpoint](#routesendendpoint)
    -   [Parameters](#parameters-1)

## ServiceKOA

**Extends Service**

HTTP server with koa

### Parameters

-   `config`  
-   `owner`  

### Properties

-   `server` **http.Server** only present if state is running
-   `koa` **koa** 

### name

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 'koa'

## RouteSendEndpoint

**Extends SendEndpoint**

Endpoint to link against a koa route

### Parameters

-   `name`  {string} endpoint name
-   `owner`  {Step} the owner of the endpoint
-   `path`  
-   `method`  {string} http method defaults to get
-   `serviceName`  {string} if present registers the route as a service

# install

With [npm](http://npmjs.org) do:

```shell
npm install kronos-service-koa
```

# license

BSD-2-Clause
