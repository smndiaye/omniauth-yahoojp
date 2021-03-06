# OmniAuth YahooJp [![Gem Version](https://badge.fury.io/rb/omniauth-yahoojp.svg)](https://badge.fury.io/rb/omniauth-yahoojp)

This is the official OmniAuth strategy for authenticating to Yahoo! JAPAN( [YConnect](http://developer.yahoo.co.jp/yconnect/) ).
To use it, you'll need to sign up for a YConnect Application ID and Secret
on the [Yahoo! JAPAN Developer Network](https://e.developer.yahoo.co.jp/dashboard/).

## Basic Usage

YConnect API v1 lets you set scopes to provide granular access to different types of data: 

    use OmniAuth::Builder do
        provider :yahoojp, ENV['YAHOOJP_KEY'], ENV['YAHOOJP_SECRET'], 
        {
            scope: "openid profile email address"
        }
    end

## Advanced Parameters

You can also set :display, :prompt, :scope, :bail parameter to specify behavior of sign-in and permission page.
More info on [YConnect](http://developer.yahoo.co.jp/yconnect/).

## License

Copyright (c) 2013 by mikanmarusan

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
