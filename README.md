[![npm](https://img.shields.io/npm/v/@kronos-integration/service-http.svg)](https://www.npmjs.com/package/@kronos-integration/service-http)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![minified size](https://badgen.net/bundlephobia/min/@kronos-integration/service-http)](https://bundlephobia.com/result?p=@kronos-integration/service-http)
[![downloads](http://img.shields.io/npm/dm/@kronos-integration/service-http.svg?style=flat-square)](https://npmjs.org/package/@kronos-integration/service-http)
[![GitHub Issues](https://img.shields.io/github/issues/Kronos-Integration/service-http.svg?style=flat-square)](https://github.com/Kronos-Integration/service-http/issues)
[![Greenkeeper](https://badges.greenkeeper.io/Kronos-Integration/service-http.svg)](https://greenkeeper.io/)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/Kronos-Integration/service-http)
[![Build Status](https://secure.travis-ci.org/Kronos-Integration/service-http.png)](http://travis-ci.org/Kronos-Integration/service-http)
[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![Known Vulnerabilities](https://snyk.io/test/github/Kronos-Integration/service-http/badge.svg)](https://snyk.io/test/github/Kronos-Integration/service-http)

# kronos-service-koa

koa backed http server

# API

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [ServiceHTTP](#servicehttp)
    -   [Properties](#properties)
    -   [extendetName](#extendetname)
    -   [endpointFactoryFromConfig](#endpointfactoryfromconfig)
        -   [Parameters](#parameters)
    -   [name](#name)
-   [HTTPEndpoint](#httpendpoint)
    -   [Parameters](#parameters-1)
-   [WSEndpoint](#wsendpoint)
    -   [Parameters](#parameters-2)
-   [authenticate](#authenticate)
    -   [Parameters](#parameters-3)
-   [CTXInterceptor](#ctxinterceptor)
    -   [name](#name-1)
-   [CTXBodyParamInterceptor](#ctxbodyparaminterceptor)
    -   [name](#name-2)
-   [CTXJWTVerifyInterceptor](#ctxjwtverifyinterceptor)
    -   [name](#name-3)

## ServiceHTTP

**Extends Service**

HTTP server

### Properties

-   `server` **http.Server** only present if state is running

### extendetName

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** name with url

### endpointFactoryFromConfig

on demand create RouteSendEndpoint´s

#### Parameters

-   `name` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 
-   `definition` **([Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object) \| [string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String))** 
-   `ic`  

Returns **Class** RouteSendEndpoint if path is present of name starts with '/'

### name

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 'http'

## HTTPEndpoint

**Extends SendEndpoint**

Endpoint to link against a http route

### Parameters

-   `name` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** endpoint name
-   `owner` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** owner of the endpoint
-   `options` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)**  (optional, default `{}`)

## WSEndpoint

**Extends SendEndpoint**

Endpoint to link against a websocket route

### Parameters

-   `name` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** endpoint name
-   `owner` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** owner of the endpoint
-   `options` **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)**  (optional, default `{}`)
    -   `options.path` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** url path defaults to endpoint name

## authenticate

check sec-websocket-protocol header for presence of
'access_token' and the token

### Parameters

-   `service` **Service** 
-   `request` **any** 

## CTXInterceptor

**Extends Interceptor**

extracts params form request body

### name

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 'ctx-body-param'

## CTXBodyParamInterceptor

**Extends Interceptor**

extracts params form request body

### name

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 'ctx-body-param'

## CTXJWTVerifyInterceptor

**Extends Interceptor**

only forward requests if a valid jwt token is present

### name

Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** 'ctx-jwt-verify'

# install

With [npm](http://npmjs.org) do:

```shell
npm install kronos-service-koa
```

# license

BSD-2-Clause
