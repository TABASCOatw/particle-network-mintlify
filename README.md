# Mintlify Starter Kit

Click on `Use this template` to copy the Mintlify starter kit. The starter kit contains examples including

- Guide pages
- Navigation
- Customizations
- API Reference pages
- Use of popular components

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

### Publishing Changes

Install our Github App to auto propagate changes from your repo to your deployment. Changes will be deployed to production automatically after pushing to the default branch. Find the link to install on your dashboard. 

#### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`

## Landing page style file

```
:root {
    font-size: 16px;
  }
  [class^="LandingWrap"] {
    width: 100% !important;
    padding: 0;
  }
  #content-head > h1 {
    margin-top: 1rem;
    margin-bottom: 4rem;
  }
  body {
    background-color: #000;
    /* overflow-x: hidden; */
  }
  .rm-LandingPage {
    max-width: 100%;
    overflow: hidden;
  }
  .rm-Header {
    background-color: #000 !important;
  }
  #content-container {
    max-width: 100%;
    overflow: hidden;
  }
  #content-head {
    font-size: 3rem;
    font-weight: 800;
    line-height: normal;
    text-align: center;
    letter-spacing: 0em;
    font-feature-settings: "kern" on;
    text-align: center;
    margin: 0;
    white-space: nowrap;
    color: #fff
  }
  .docs {
    width: 100%;
  }
  .cards {
    width: 84rem;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    row-gap: 2.75rem;
  }

  .service-card {
    z-index: 10;
    display: flex;
    flex-direction: column;
    width: 25.875rem;
    height: 24rem;
    padding: 1.75rem;
    border-radius: 1.875rem;
    background: #34013f;
    transition: all .3s linear;
  }

  .service-card:hover {
    background-color: #000;
    box-shadow: 0px 4px 24px 0px #B700FF;
    transform: translate(-4px, -4px);
  }

  .service-card .title {
    margin-bottom: 1rem;
    font-weight: bold;
    font-size: 2rem;
    line-height: normal;
    white-space: nowrap;
    letter-spacing: 0;
    color: #fff;
  }
  .content {
    flex: 1;
    font-weight: 300;
    font-size: 1.5rem;
    line-height: normal;
    letter-spacing: 0;
    color: #fff;
  }

  .footer {
    display: flex;
    justify-content: space-between;
    align-items: end;
  }
  .icon-wrapper {
    width: 6.25rem;
    height: 6.25rem;
  }

  .icon-wrapper > svg {
    width: 6.25rem;
    height: 6.25rem;
  }

  .icon {
    width: 100%;
    height: 100%;
  }

  .link {
    display: inline-block;
    height: 1.5rem;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none !important;
    gap: 0px;
    font-size: 1.5rem;
    font-weight: 500;
    color: #AD44FF !important;
    transform: translateY(-1.5rem);
  }

  .learn-more-text {
    transform: translateY(-1px);
  }
  .octicon {
    width: 1.5rem;
    height: 1.5rem;
    transition: transform 0.2s;
    transform: translateX(0);
  }
  .octicon-chevrow-stem {
    stroke-dasharray: 10;
    stroke-dashoffset: 10;
    transition: stroke-dashoffset 0.2s;
  }

  a:hover > svg {
    transform: translateX(.5rem);
  }

  a:hover > svg > .octicon-chevrow-stem {
    stroke-dashoffset: 20;
  }

  .learn-more-text {
    width: 100%;
    position: relative;
  }

  .learn-more-text::after {
    content: '';
    position: absolute;
    width: calc(100% + 1.25rem);
    transition: transform 0.3s ease;
    border-bottom: 2px solid #AD44FF;
    transform: scaleX(0);
    pointer-events: none;
    left: 0;
    bottom: 0;
    transform-origin: 0 0;
  }

  .learn-more-text:hover::after {
    transform: scaleX(1);
  }

  .other-products {
    height: 12.5rem;
  }

  .other-products-title {
    font-size: 64px;
    font-weight: 800;
    line-height: normal;
    text-align: center;
    letter-spacing: 0em;
    font-feature-settings: "kern" on;
    color: #FFFFFF;
    text-align: center;
    margin-top: 5rem;
    margin-bottom: 5rem;
    position: relative;
    z-index: 200;
  }

  .other-products-list {
    display: flex;
    justify-content: space-between;
    width: 82rem;
    margin: 0 auto;
    align-items: center;
    position: relative;
    z-index: 200;
  }

  .other-products-link {
    font-size: 24px;
    font-weight: normal;
    line-height: normal;
    text-align: center;
    letter-spacing: 0em;
    font-feature-settings: "kern" on;
    color: #FFFFFF;
    text-decoration: none !important;
    width: auto;
    position: relative;
  }

  .other-products-link::after {
    content: '';
    position: absolute;
    width: 100%;
    transition: transform 0.3s ease;
    border-bottom: 2px solid #fff;
    transform: scaleX(0);
    pointer-events: none;
    left: 0;
    bottom: 0;
    transform-origin: 0 0;
  }

  .other-products-link:hover::after {
    content: '';
    position: absolute;
    width: 100%;
    transition: transform 0.3s ease;
    border-bottom: 2px solid #fff;
    transform: scaleX(1);
    pointer-events: none;
    left: 0;
    bottom: 0;
    transform-origin: 0 0;
  }

  .dot {
    width: .625rem;
    height: .625rem;
    border-radius: 50%;
    background-color: #fff;
  }

  .chains {
    width: 100%;
    height: 98.125rem;
    position: relative;
  }

  .chains > .animation-chains {
    width: 90rem;
    height: auto;
    margin: 0 auto;
    display: block;
    position: relative;
    z-index: 200;
  }

  .chains > .animation-background {
    position: absolute;
    width: 90rem;
    height: auto;
    margin: 0 auto;
    display: block;
    top: 0;
    left: 50%;
    transform: translateX(-45rem);
    z-index: 100;
  }

  /* .chains > .chains-video {
    width: 90rem;
    display: block;
    margin: 0 auto;
  } */
  .sponsors {
    width: 100%;
    position: relative;
    margin-bottom: 7.5rem;
    z-index: 200;
  }
  .sponsors-title {
    font-size: 3.125rem;
    font-weight: 800;
    line-height: normal;
    letter-spacing: 0em;
    font-feature-settings: "kern" on;
    background: linear-gradient(90deg, #E85FD4 0%, #685FEE 99%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    width: 100%;
    text-align: center;
  }
  .sponsors-img {
    width: 90rem;
    height: auto;
    margin: 0 auto;
  }
  .sponsors-img>img {
    width: 100%;
    height: auto;
  }

  .plug {
    width: 100%;
    margin-bottom: 1.25rem;
    height: 37.5rem;
    position: relative;
    z-index: 2;
    background: url('https://files.readme.io/c9195ea-poster1.png') no-repeat;
    background-size: 100% 100%;
  }

  .plug-logo {
    width: 7.5rem;
    height: 7.5rem;
    margin: 0 auto;
    position: relative;
    z-index: 200;
  }

  .plug-logo>img {
    width: 100%;
    height: 100%;
    position: relative;
    z-index: 200;
  }

  .footer-video {
    width: 100%;
    height: calc(100vw * 0.56);
    position: absolute;
    bottom: 0px;
    left: 0;
    z-index: 1;
    opacity: 0.7;
  }

  .animation-text {
    width: 50rem;
    height: 7.5rem;
    margin: 0 auto;
    position: relative;
    z-index: 200;
  }

  .animation-text>img {
    width: 100%;
    height: 100%;
  }
  
  .footer-container {
    position: relative;
    width: 90rem;
    margin: 0 auto;
  }

  .wrapper {
    color: #fff;
    width: 75rem;
    margin: auto;
  }

  .row-1 {
    display: flex;
    padding-bottom: 6.25rem;
  }

  .col {
    flex: 1;
    text-align: left;
  }

  .col-1 {
    width: 25.625rem;
    margin-right: 8.75rem;
    flex: none;
  }

  .col-2 {
    min-width: 15rem;
  }
  
  .logo {
    width: 14.375rem;
    margin-bottom: 1.5rem;
  }

  .logo>img {
    width: 100%;
  }
  .icons {
    display: flex;
    gap: 1.25rem;
  }

  .icons> a > img {
    width: 2rem;
    height: 2rem;
  }

  .copy-write {
    font-size: .875rem;
    font-weight: 500;
    line-height: 50px;
    color: #848398;
    margin-top: 16px;
  }

  .title {
    font-size: 1rem;
    font-weight: 400;
    color: #ffffff;
    line-height: 1.3;
    margin-bottom: 1rem;
  }
  .item {
    font-size: .875rem;
    font-weight: 400;
    line-height: 3;
  }

  .item > a {
    color: #848398 !important;
    text-decoration: none !important;
  }

  .item > a:hover {
    color: #fff !important;
  }
  .row-3 {
    display: flex;
    justify-content: center;
  }
  .footer-icon {
    display: flex;
    justify-content: center;
    width: 62.5rem;
    height: 6.25rem;
    position: relative;
  }
  .bg-content {
    width: 62.5rem;
    height: 6.25rem;
    max-width: 100vw;
    position: absolute;
    top: 0px;
    overflow: hidden;
    z-index: 0;
  }

  .wrap {
    width: 62.5rem;
    max-width: 100vw;
    height: 12.5rem;
    display: flex;
    justify-content: center;
  }

  .wrap > img {
    width: auto;
    height: 100%;
    position: relative;
  }

  .img {
    position: absolute;
    width: 2.875rem;
    left: 50%;
    top: 2.5rem;
    transform: translateX(-50%);
    z-index: 2;
  }

  .img > img {
    width: 100%;
  }

  .halo-top-right {
    position: absolute;
    z-index: 0;
    width: 50rem;
    height: 50rem;
    pointer-events: none;
    top: 0;
    right: 0;
  }
  .halo-top-right::after {
    position: absolute;
    top: -43.75rem;
    right: -43.75rem;
    width: 75rem;
    height: 75rem;
    background: radial-gradient(50% 50% at 50% 50%, #002ED2 0%, rgba(103, 0, 162, 0) 99%);
    content: '';
    pointer-events: none;
  }

  .halo-top-left {
    position: absolute;
    z-index: 0;
    width: 50rem;
    height: 50rem;
    pointer-events: none;
    top: 0;
    left: 0;
  }

  .halo-top-left::after {
    position: absolute;
    top: -43.75rem;
    left: -43.75rem;
    width: 75rem;
    height: 75rem;
    background: radial-gradient(50% 50% at 50% 50%, rgba(198, 5, 185, 0.8784) 0%, rgba(0, 22, 128, 0) 100%);
    content: '';
    pointer-events: none;
  }

  .halo-middle-left {
    position: absolute;
    z-index: 0;
    width: 50rem;
    height: 50rem;
    pointer-events: none;
    top: 12.5rem;
    left: 0;
  }

  .halo-middle-left::after {
    position: absolute;
    top: -37.5rem;
    left: -37.5rem;
    width: 62.5rem;
    height: 62.5rem;
    background: radial-gradient(50% 50% at 50% 50%, rgba(20, 103, 77, 0.8784) 0%, rgba(0, 22, 128, 0) 100%);
    content: '';
    pointer-events: none;
  }

  .halo-bottom-left {
    position: absolute;
    z-index: 0;
    width: 50rem;
    height: 50rem;
    pointer-events: none;
    top: 12.5rem;
    left: 0;
  }

  .halo-bottom-left::after {
    position: absolute;
    top: 0px;
    left: -37.5rem;
    width: 62.5rem;
    height: 1000px;
    background: radial-gradient(50% 50% at 50% 50%, #002ED2 0%, rgba(103, 0, 162, 0) 99%);
    content: '';
    pointer-events: none;
  }

  .halo-bottom-right {
    position: absolute;
    z-index: 0;
    width: 50rem;
    height: 50rem;
    pointer-events: none;
    top: 12.5rem;
    right: 0;
  }

  .halo-bottom-right::after {
    position: absolute;
    top: -37.5rem;
    right: -37.5rem;
    width: 62.5rem;
    height: 62.5rem;
    background: radial-gradient(50% 50% at 50% 50%, rgba(198, 5, 185, 0.8784) 0%, rgba(0, 22, 128, 0) 100%);
    content: '';
    pointer-events: none;
  }

  .item-aa-mobile {
    display: none;
  }
  @media screen and (min-width: 800px) and (max-width: 1920px) {
    :root {
      font-size: calc(100vw / 100 - 4px);
    }
  }
  @media screen and (max-width: 800px) {
    :root {
      font-size: 12px;
      width: 100vw;
    }

    .cards {
      width: 94vw;
    }

    .service-card {
      width: 14.6rem;
      height: 16rem;
    }

    .service-card > .title {
      font-size: 1.2rem;
    }

    .service-card > .content {
      font-size: 0.8rem;
    }
    .link {
      font-size: 1rem;
      transform: translateY(-0.4rem);
    }

    .icon-wrapper {
      width: 3rem;
      height: 3rem;
    }

    .icon-wrapper > svg {
      width: 3rem;
      height: 3rem;
    }


    .other-products-title {
      font-size: 2rem;
      margin-bottom: 2rem;
    }
    
    .other-products-list {
      width: 90vw;
      flex-direction: column;
      gap: 1.25rem;
    }

    .other-products-link {
      font-size: 1.125rem;
    }

    .dot {
      display: none;
    }

    .chains {
      height: auto;
    }
    .item-aa-mobile {
      display: block;
    }

    .chains > .animation-chains {
      width: 100vw;
      margin: 0 auto;
    }

    .chains > .animation-background {
      width: 100vw;
      top: 0;
      left: 0;
      transform: none;
    }

    /* .chains > .chains-video {
      width: 100vw;
      margin: 0 auto;
    } */

    .sponsors-title {
      font-size: 2rem;
      position: relative;
      z-index: 200;
    }

    .sponsors-img {
      width: 90vw;
      height: 30vw;
      margin: 0 auto;
    }

    .sponsors-img > img {
      height: auto;
    }

    .plug {
      height: 20rem;
    }

    .animation-text {
      width: 90vw;
      height: 20vw;
      margin: 0 auto;
    }

    .animation-text >img {
      height: auto;
    }

    .footer-video {
      z-index: 0;
      bottom: 0;
      width: 100vw;
      height: calc(100vw * 0.56);
      left: 50%;
      transform: translateX(-50%);
    }

    .footer-container {
      width: 100vw;
    }

    .wrapper {
      width: 100vw;
      padding: 20px 20px;
      padding-bottom: 0;
      position: relative;
      z-index: 200;
    }

    .col-1 {
      position: absolute;
      display: none;
    }

    .col-2 {
      min-width: 32%;
    }

    .col-2  .item {
      white-space: nowrap;
    }

    .col-4 {
      flex: 1;
    }

    .col-4  .item {
      white-space: nowrap;
    }

    .title {
      font-size: 0.9rem;
      margin-bottom: 1rem;
    }

    .item {
      font-size: 0.7rem;
      line-height: 1.4;
    }

    .item-aa {
      display: none;
    }

    .halo-bottom-right {
      display: none;
    }

    #content-head {
      font-size: 1rem;
      position: relative;
      z-index: 200;
    }
    .halo-middle-left {
      top: 2rem;
    }
  }
  ```

  ## Landing page HTML

  ```
  ---
title: Explore Our Products
mode: "wide"
---

import React from "react";
import './style.css';

export default function Gallery() {
    return (
        <>
            <header id="content-head">
                <h1>Explore Our Products</h1>
            </header>
            <div className="halo-top-right"></div>
            <div className="halo-top-left"></div>
            <div id="docs" className="docs">
                <div className="cards">
                    <div className="service-card">
                        <div className="title">Account Abstraction</div>
                        <div className="content">Modularly tap into ERC-4337 AA within your dApp. Leverage Particle’s Bundler, Paymaster, and compatibility with Smart Account implementations.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-smart-waas">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M79.2652,23L19.7348,23C16.02123,23,13.0000000900738,26.03632,13.0000000900738,29.768430000000002L13,71.2316C13,74.96379999999999,16.02123,78,19.7348,78L79.2652,78C82.9789,78,86,74.9637,86,71.2316L86,29.768430000000002C86,26.03624,82.9788,23,79.2652,23ZM19.7348,27.93254L79.2652,27.93254C80.2726,27.93254,81.092,28.75612,81.092,29.768430000000002L81.092,35.696L17.90803,35.696L17.90803,29.768430000000002C17.90803,28.75612,18.72752,27.93254,19.7348,27.93254ZM79.2652,73.0675L19.7348,73.0675C18.72752,73.0675,17.90803,72.2438,17.90803,71.2316L17.90803,39.9075L81.092,39.9075L81.092,71.2316C81.092,72.2439,80.2726,73.0675,79.2652,73.0675Z" fill="#AD44FF"></path>
                                    <path d="M74.5898,50L61.4102,50C60.08458,50,59,48.87502,59,47.5C59,46.12498,60.08458,45,61.4102,45L74.5898,45C75.9154,45,77,46.12498,77,47.5C77,48.87502,75.9154,50,74.5898,50Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div className="service-card">
                        <div className="title">Particle Auth</div>
                        <div className="content">Onboard users in one click through a Web 2.0-adjacent interface. Compatible with phone, email, Google, X, and many more.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-particle-auth">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M49.9966,21.32759C50.1318,21.32759,50.2602,21.34757,50.3886,21.387520000000002C50.3886,21.387520000000002,72.62610000000001,28.027,72.62610000000001,28.027C73.2007,28.200200000000002,73.58590000000001,28.713,73.58590000000001,29.299C73.58590000000001,29.299,73.58590000000001,57.6351,73.58590000000001,57.6351C73.58590000000001,60.3322,72.8289,62.976,71.40270000000001,65.2735C69.97659999999999,67.5777,67.9353,69.44239999999999,65.50200000000001,70.67439999999999C65.50200000000001,70.67439999999999,49.9966,78.5059,49.9966,78.5059C49.9966,78.5059,34.498,70.67439999999999,34.498,70.67439999999999C32.0647,69.44239999999999,30.02342,67.5777,28.59725,65.2735C27.17108,62.9693,26.41405,60.3322,26.41405,57.6351C26.41405,57.6351,26.41405,29.299,26.41405,29.299C26.41405,28.7063,26.79932,28.1935,27.37385,28.027C27.37385,28.027,49.6113,21.387520000000002,49.6113,21.387520000000002C49.733000000000004,21.34757,49.8682,21.32759,49.9966,21.32759ZM49.9966,16C49.334199999999996,16,48.6786,16.0932328,48.036500000000004,16.286358C48.036500000000004,16.286358,25.79897,22.92586,25.79897,22.92586C22.94663,23.77828,21,26.3622,21,29.299C21,29.299,21,57.6351,21,57.6351C21,65.12700000000001,25.25825,71.99289999999999,32.024100000000004,75.4093C32.024100000000004,75.4093,48.151399999999995,83.5605,48.151399999999995,83.5605C48.7327,83.8535,49.367999999999995,84,50.0034,84C50.6387,84,51.274100000000004,83.8535,51.8554,83.5605C51.8554,83.5605,67.9759,75.4159,67.9759,75.4159C74.74170000000001,71.9996,79,65.1337,79,57.6418C79,57.6418,79,29.299,79,29.299C79,26.3622,77.05340000000001,23.77828,74.201,22.92586C74.201,22.92586,51.963499999999996,16.286359,51.963499999999996,16.286359C51.3214,16.0932335,50.659,16.000000713264,49.9966,16.000000713264C49.9966,16.000000713264,49.9966,16,49.9966,16Z" fill="#AD44FF"></path>
                                    <path d="M47.3858,63C46.686800000000005,63,45.981,62.7355,45.4464,62.2065C45.4464,62.2065,37.0171,53.8644,37.0171,53.8644C35.9481,52.8064,35.9481,51.0905,37.0171,50.025800000000004C38.086200000000005,48.961,39.82,48.9677,40.896,50.025800000000004C40.896,50.025800000000004,47.3858,56.4484,47.3858,56.4484C47.3858,56.4484,63.1273,40.8699,63.1273,40.8699C64.1964,39.8118,65.9302,39.8118,67.0062,40.8699C68.0821,41.9279,68.0752,43.6438,67.0062,44.7085C67.0062,44.7085,49.3253,62.2065,49.3253,62.2065C48.7839,62.7355,48.0848,63,47.3858,63C47.3858,63,47.3858,63,47.3858,63ZM75.2573,38.6928C74.99680000000001,38.6928,74.7296,38.652100000000004,74.4623,38.5775C74.4623,38.5775,51.251000000000005,31.61223,51.251000000000005,31.61223C50.4354,31.36807,49.5651,31.36807,48.7496,31.61223C48.7496,31.61223,25.53825,38.5707,25.53825,38.5707C24.09226,39.0048,22.557169000000002,38.1977,22.118572,36.7599C21.679976,35.32206,22.495492,33.80964,23.94834,33.37558C23.94834,33.37558,47.1597,26.4171,47.1597,26.4171C49.0169,25.860967,50.9837,25.860967,52.840900000000005,26.4171C52.840900000000005,26.4171,76.0522,33.37558,76.0522,33.37558C77.4982,33.80964,78.3206,35.32206,77.882,36.7599C77.5188,37.9332,76.436,38.6928,75.2573,38.6928C75.2573,38.6928,75.2573,38.6928,75.2573,38.6928Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div className="service-card">
                        <div className="title">Embedded Wallet</div>
                        <div className="content">A Web3 wallet, right within your dApp. Allow your users to focus on your product rather than navigating a typical wallet.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-particle-wallet">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M72.037,20L27.963,20C20.83333,20,15,25.71875,15,32.7083L15,68.29169999999999C15,75.2812,20.83333,81,27.963,81L72.037,81C79.1667,81,85,75.2812,85,68.29169999999999L85,32.7083C85,25.71875,79.1667,20,72.037,20ZM79.8148,58.125L56.4815,58.125C52.2037,58.125,48.7037,54.6937,48.7037,50.5C48.7037,46.3063,52.2037,42.875,56.4815,42.875L79.8148,42.875L79.8148,58.125ZM56.4815,37.7917C49.3519,37.7917,43.5185,43.510400000000004,43.5185,50.5C43.5185,57.4896,49.3519,63.2083,56.4815,63.2083L79.8148,63.2083L79.8148,68.29169999999999C79.8148,72.4854,76.31479999999999,75.91669999999999,72.037,75.91669999999999L27.963,75.91669999999999C23.685180000000003,75.91669999999999,20.18519,72.4854,20.18519,68.29169999999999L20.18519,32.7083C20.18519,28.514580000000002,23.685180000000003,25.08333,27.963,25.08333L72.037,25.08333C76.31479999999999,25.08333,79.8148,28.514580000000002,79.8148,32.7083L79.8148,37.7917L56.4815,37.7917Z" fill="#AD44FF"></path>
                                    <path d="M59.333330000000004,50.5Q59.333330000000004,50.62896,59.32049,50.7573Q59.30765,50.88563,59.28209,51.01211Q59.25654,51.13859,59.21851,51.262Q59.18048,51.3854,59.130340000000004,51.50454Q59.08021,51.623689999999996,59.01846,51.73742Q58.9567,51.85115,58.88392,51.95837Q58.81114,52.0656,58.728030000000004,52.16528Q58.64492,52.26497,58.552279999999996,52.35615Q58.459649999999996,52.44734,58.35838,52.52915Q58.25711,52.61096,58.14819,52.68261Q58.03926,52.75425,57.92372,52.815039999999996Q57.80819,52.87583,57.68716,52.92518Q57.56612,52.97453,57.44076,53.01197Q57.3154,53.0494,57.18691,53.07456Q57.05842,53.09972,56.92805,53.11236Q56.79767,53.125,56.666669999999996,53.125Q56.53566,53.125,56.40529,53.11236Q56.27491,53.09972,56.14643,53.07456Q56.01794,53.0494,55.89257,53.01197Q55.76721,52.97453,55.64618,52.92518Q55.52514,52.87583,55.40961,52.815039999999996Q55.29407,52.75425,55.18515,52.68261Q55.07622,52.61096,54.974951,52.52915Q54.873683,52.44734,54.781049,52.35615Q54.688414,52.26497,54.605305,52.16528Q54.522197,52.0656,54.449414,51.95837Q54.376632,51.85115,54.314877,51.73742Q54.253121,51.623689999999996,54.202988,51.50454Q54.152854,51.3854,54.114826,51.262Q54.076797,51.13859,54.0512392,51.01211Q54.0256815,50.88563,54.0128407,50.7573Q54,50.62896,54,50.5Q54,50.37104,54.0128407,50.24271Q54.0256815,50.11437,54.0512392,49.98789Q54.076797,49.86141,54.114826,49.738Q54.152854,49.6146,54.202988,49.49546Q54.253121,49.37631,54.314877,49.26258Q54.376632,49.14885,54.449414,49.04163Q54.522197,48.9344,54.605305,48.834718Q54.688414,48.735032,54.781049,48.643845Q54.873683,48.552658,54.974951,48.470848Q55.07622,48.389037,55.18515,48.317392Q55.29407,48.245747,55.40961,48.184957Q55.52514,48.124166,55.64618,48.074816Q55.76721,48.025466,55.89257,47.988032Q56.01794,47.9505971,56.14643,47.9254386Q56.27491,47.9002802,56.40529,47.8876401Q56.53566,47.875,56.666669999999996,47.875Q56.79767,47.875,56.92805,47.8876401Q57.05842,47.9002802,57.18691,47.9254386Q57.3154,47.9505971,57.44076,47.988032Q57.56612,48.025466,57.68716,48.074816Q57.80819,48.124166,57.92372,48.184957Q58.03926,48.245747,58.14819,48.317392Q58.25711,48.389037,58.35838,48.470848Q58.459649999999996,48.552658,58.552279999999996,48.643845Q58.64492,48.735032,58.728030000000004,48.834718Q58.81114,48.9344,58.88392,49.04163Q58.9567,49.14885,59.01846,49.26258Q59.08021,49.37631,59.130340000000004,49.49546Q59.18048,49.6146,59.21851,49.738Q59.25654,49.86141,59.28209,49.98789Q59.30765,50.11437,59.32049,50.24271Q59.333330000000004,50.37104,59.333330000000004,50.5Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div className="service-card">
                        <div className="title">Particle Connect</div>
                        <div className="content">Connect to both Web 2.0 accounts and mainstream wallets, enhancing accessibility through a unified interface.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-particle-connect">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M21.177970000000002,52.3162L21.177970000000002,23.67521C21.177970000000002,22.264960000000002,22.33529,21.11966,23.76695,21.11966L62.2416,21.11966C63.6733,21.11966,64.8306,22.264960000000002,64.8306,23.67521L64.8306,52.3248C64.8306,53.735,63.6733,54.8803,62.2416,54.8803L49.1253,54.8803C47.8393,54.8803,46.7935,55.9231,46.7935,57.2051L46.7935,57.6752C46.7935,58.9573,47.8393,60,49.1253,60L64.822,60C67.6768,60,70,57.7094,70,54.8803L70,21.11966C70,18.2906,67.6853,16,64.822,16L18.58898,16C17.15733,16,16,17.1453,16,18.55556L16,54.8718C16,57.7009,18.31465,59.9915,21.177970000000002,59.9915L23.76695,59.9915C25.05287,59.9915,26.0987,58.9487,26.0987,57.6667L26.0987,57.1966C26.0987,55.9145,25.05287,54.8718,23.76695,54.8718C22.33529,54.8803,21.177970000000002,53.735,21.177970000000002,52.3162Z" fill="#AD44FF"></path>
                                    <path d="M79.75200000000001,40L77.128,40C75.9724,40,75.0253,40.944056,75.0253,42.11538L75.0253,43.12063C75.0253,44.28322,75.9637,45.23601,77.128,45.23601C78.57900000000001,45.23601,79.75200000000001,46.40734,79.75200000000001,47.84965L79.75200000000001,77.1503C79.75200000000001,78.59270000000001,78.57900000000001,79.76400000000001,77.128,79.76400000000001L37.87204,79.76400000000001C36.42101,79.76400000000001,35.24803,78.59270000000001,35.24803,77.1503L35.24803,47.84965C35.24803,46.40734,36.42101,45.23601,37.87204,45.23601L51.687200000000004,45.23601C52.8428,45.23601,53.7899,44.29196,53.7899,43.12063L53.7899,42.11538C53.7899,40.952797,52.8515,40,51.687200000000004,40L35.24803,40C32.35466,40,30,42.34266,30,45.23601L30,79.76400000000001C30,82.65729999999999,32.34597,85,35.24803,85L79.75200000000001,85C82.64529999999999,85,85,82.65729999999999,85,79.76400000000001L85,45.23601C85,42.34266,82.654,40,79.75200000000001,40Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div className="service-card">
                        <div className="title">BTC Connect</div>
                        <div className="content">The first account abstraction protocol for Bitcoin. Control a Smart Account on an EVM-compatible L2 using your Bitcoin wallet.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-btc-connect">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M50.5,13C29.7893,13,13,29.7893,13,50.5C13,71.2107,29.7893,88,50.5,88C71.2107,88,88,71.2107,88,50.5C87.9898,29.7936,71.2064,13.010243,50.5,13ZM50.5,18.19802C68.3399,18.19802,82.802,32.6601,82.802,50.5C82.802,68.3399,68.3399,82.802,50.5,82.802C32.6601,82.802,18.19802,68.3399,18.19802,50.5C18.20826,32.6643,32.6644,18.20826,50.5,18.19802ZM67.5792,42.8886C67.5792,37.7622,63.4234,33.6064,58.297,33.6064L55.698,33.6064L55.698,30.2649C55.7677,29.2121,54.8944,28.3388,53.8416,28.4084L52.3564,28.4084C51.3037,28.3388,50.4304,29.2121,50.5,30.2649L50.5,33.6064L45.302,33.6064L45.302,30.2649C45.3716,29.2121,44.4983,28.3388,43.445499999999996,28.4084L41.9604,28.4084C40.9076,28.3388,40.0343,29.2121,40.104,30.2649L40.104,33.6064L35.0916,33.6064C34.038799999999995,33.5368,33.1655,34.4101,33.2352,35.462900000000005L33.2352,36.948C33.1655,38.0008,34.038799999999995,38.8741,35.0916,38.804500000000004L40.104,38.804500000000004L40.104,61.0817L35.0916,61.0817C34.038799999999995,61.012,33.1655,61.8853,33.2352,62.9381L33.2352,64.4233C33.1655,65.4761,34.038799999999995,66.3494,35.0916,66.27969999999999L40.104,66.27969999999999L40.104,69.0644C40.0343,70.1171,40.9076,70.9904,41.9604,70.9208L43.445499999999996,70.9208C44.4983,70.9904,45.3716,70.1171,45.302,69.0644L45.302,65.7228L50.5,65.7228L50.5,69.0644C50.4304,70.1171,51.3037,70.9904,52.3564,70.9208L53.8416,70.9208C54.8944,70.9904,55.7677,70.1171,55.698,69.0644L55.698,65.7228L58.297,65.7228C63.4234,65.7228,67.5792,61.567,67.5792,56.4406C67.5467,53.8461,66.47710000000001,51.3725,64.6089,49.5718C66.4306,47.8152,67.4961,45.4179,67.5792,42.8886ZM58.1114,60.7104L45.302,60.7104L45.302,52.1708L58.297,52.1708C60.6725,52.1284,62.6093,54.0651,62.5668,56.4406C62.4579,58.8243,60.4975,60.703,58.1114,60.7104ZM58.1114,47.1584L45.302,47.1584L45.302,38.6188L58.297,38.6188C60.6725,38.5764,62.6093,40.5131,62.5668,42.8886C62.5161,45.2983,60.521,47.2102,58.1114,47.1584Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                    <div className="service-card">
                        <div className="title">Web3 Services</div>
                        <div className="content">Access to Node services, NFT capabilities, data APIs, fiat on-ramps and much more.</div>
                        <div className="footer">
                            <div className="learn-more">
                                <a className="link" target="_self" href="https://developers.particle.network/reference/introduction-to-web3-services">
                                    <div className="learn-more-text">learn more</div>
                                    <svg className="octicon arrow-symbol-mktg" fill="none" height="16" viewBox="0 0 16 16" width="16" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M7.28033 3.21967C6.98744 2.92678 6.51256 2.92678 6.21967 3.21967C5.92678 3.51256 5.92678 3.98744 6.21967 4.28033L7.28033 3.21967ZM11 8L11.5303 8.53033C11.8232 8.23744 11.8232 7.76256 11.5303 7.46967L11 8ZM6.21967 11.7197C5.92678 12.0126 5.92678 12.4874 6.21967 12.7803C6.51256 13.0732 6.98744 13.0732 7.28033 12.7803L6.21967 11.7197ZM6.21967 4.28033L10.4697 8.53033L11.5303 7.46967L7.28033 3.21967L6.21967 4.28033ZM10.4697 7.46967L6.21967 11.7197L7.28033 12.7803L11.5303 8.53033L10.4697 7.46967Z" fill="currentColor"></path>
                                        <path className="octicon-chevrow-stem" d="M1.75 8H11" stroke="currentColor"></path>
                                    </svg>
                                </a>
                            </div>
                            <div className="icon-wrapper">
                                <svg xmlns="http://www.w3.org/2000/svg" fill="none" width="100" height="100" viewBox="0 0 100 100">
                                    <path d="M19.08128611776553,19.082857511458993C11.17895611776553,26.981937511458995,19.08128611776553,46.75743751145899,35.99842611776553,63.92303751145899L36.53482611776553,64.464437511459C53.825526117765534,81.75183751145899,73.93512611776552,89.90423751145899,81.91812611776552,81.91633751145899C89.90112611776553,73.928437511459,81.75192611776554,53.82543751145899,64.46452611776553,36.53473751145899C47.17552611776553,19.249067511458993,27.06752611776553,11.094957511458993,19.08128611776553,19.082857511458993ZM62.13602611776553,38.863337511458994C78.26642611776553,54.99383751145899,85.74262611776552,73.43813751145899,79.58952611776553,79.591137511459C73.50732611776553,85.675037511459,55.40202611776553,78.43093751145899,39.40152611776553,62.670737511458995L38.86342611776553,62.137537511458994C22.73294611776553,46.00703751145899,15.25683911776553,27.562837511458994,21.409856117765532,21.40977751145899C27.493726117765533,15.324230511458993,45.59902611776553,22.56994751145899,61.59782611776553,38.32853751145899L62.13602611776553,38.863337511458994Z" fill="#AD44FF"></path>
                                    <path d="M36.5363,36.5347C19.24239,53.8303,11.09321,73.9268,19.08111,81.918C26.4832,89.32,44.3301,82.8988,60.8341,67.90379999999999L62.0881,66.765L60.9131,65.54560000000001C59.6846,64.2599,59.7109,62.2274,60.9723,60.974C62.2253,59.7121,64.2578,59.685,65.54390000000001,60.9131L66.765,62.0881L67.90379999999999,60.8341C82.8988,44.3301,89.32,26.4832,81.918,19.08114C73.92840000000001,11.09324,53.8303,19.24241,36.5363,36.5347ZM79.7902,21.617060000000002C84.8998,27.232,79.64529999999999,42.3076,66.95920000000001,56.9406L66.4474,57.5264L66.37989999999999,57.4869C63.8278,56.1287,60.6876,56.599,58.6454,58.6454L58.392,58.912C56.5529,60.9647,56.1914,63.9473,57.4869,66.37989999999999L57.5264,66.4474L57.5116,66.4605C42.5149,79.67,26.9193,85.1006,21.406390000000002,79.59270000000001C15.320843,73.5022,22.56492,55.4068,38.3284,39.401399999999995L38.863299999999995,38.861599999999996C54.9987,22.72787,73.43469999999999,15.253404,79.59100000000001,21.408070000000002L79.7885,21.617060000000002L79.7902,21.617060000000002Z" fill="#AD44FF"></path>
                                    <path d="M58.393827858886716,58.910371066894534C56.19502985888672,61.35896106689453,56.15278385888672,65.05836106689453,58.29509785888672,67.55648106689453L58.41686785888672,67.68978106689453L58.43990785888672,67.72278106689453C58.50902785888672,67.81658106689453,58.58636785888672,67.89718106689453,58.67358785888672,67.98108106689453C61.22102785888672,70.52858106689453,65.37954785888672,70.52858106689453,67.95491785888672,67.95478106689453C70.42981785888672,65.48424106689453,70.53831785888671,61.508891066894535,68.20181785888671,58.90709106689453L67.87101785888672,58.56479106689453L67.70971785888672,58.43315106689453L67.82991785888672,58.54340106689453C65.25236785888671,56.070091066894534,61.16919785888672,56.11546006689453,58.64726785888672,58.64543106689453L58.39383785888672,58.91203106689453L58.393827858886716,58.910371066894534ZM65.72676785888672,61.08754106689453L65.73664785888673,61.09248106689453L65.62638785888672,60.97235106689453C66.91601785888672,62.25626106689453,66.91601785888672,64.34393106689453,65.62638785888672,65.62784106689453L65.41738785888671,65.82038106689453C64.19478785888671,66.85278106689454,62.40577785888672,66.85278106689454,61.18317785888672,65.82038106689453L61.09760785888672,65.74139106689454L60.91329785888672,65.54392106689453C59.68387785888672,64.25856106689453,59.71022785888672,62.22542106689453,60.97253785888672,60.97235106689453C62.22616785888672,59.70984106689453,64.25983785888673,59.68350106689453,65.54575785888672,60.91311106689453L65.72676785888672,61.08754106689453Z" fill="#AD44FF"></path>
                                    <path d="M35.405,54L33.26,46.967L34.989,46.980000000000004L36.263,51.166L37.5565,46.980000000000004L39.0255,46.980000000000004L40.319,51.166L41.593,46.980000000000004L43.322,46.980000000000004L41.177,54L39.825,54L38.291,49.424L36.757,54L35.405,54ZM47.495,54.195Q46.416,54.195,45.5938,53.7303Q44.7715,53.2655,44.3068,52.4497Q43.842,51.634,43.842,50.581Q43.842,49.4305,44.297,48.579Q44.752,47.7275,45.551500000000004,47.25625Q46.351,46.785,47.391,46.785Q48.496,46.785,49.2695,47.305Q50.043,47.825,50.4135,48.7675Q50.784,49.71,50.673500000000004,50.984L48.925,50.984L48.925,50.334Q48.925,49.2615,48.5838,48.79025Q48.2425,48.319,47.469,48.319Q46.5655,48.319,46.1398,48.86825Q45.714,49.417500000000004,45.714,50.49Q45.714,51.4715,46.1398,52.0077Q46.5655,52.544,47.391,52.544Q47.911,52.544,48.2815,52.3165Q48.652,52.089,48.847,51.66L50.614999999999995,52.167Q50.2185,53.129,49.3638,53.662Q48.509,54.195,47.495,54.195ZM45.168,50.984L45.168,49.671L49.822,49.671L49.822,50.984L45.168,50.984ZM55.581,54.195Q54.5345,54.195,53.832499999999996,53.707499999999996Q53.1305,53.22,52.7763,52.3815Q52.422,51.543,52.422,50.49Q52.422,49.437,52.772999999999996,48.5985Q53.123999999999995,47.76,53.8065,47.2725Q54.489000000000004,46.785,55.489999999999995,46.785Q56.4975,46.785,57.245000000000005,47.266Q57.9925,47.747,58.4053,48.58225Q58.818,49.417500000000004,58.818,50.49Q58.818,51.543,58.4118,52.3815Q58.0055,53.22,57.2775,53.707499999999996Q56.549499999999995,54.195,55.581,54.195ZM52.123000000000005,54L52.123000000000005,44.64L53.903999999999996,44.64L53.903999999999996,49.19L53.683,49.19L53.683,54L52.123000000000005,54ZM55.295,52.622Q55.867000000000004,52.622,56.231,52.336Q56.595,52.05,56.7705,51.565799999999996Q56.946,51.0815,56.946,50.49Q56.946,49.905,56.763999999999996,49.42075Q56.582,48.9365,56.2018,48.64725Q55.8215,48.358000000000004,55.230000000000004,48.358000000000004Q54.677499999999995,48.358000000000004,54.3363,48.6245Q53.995000000000005,48.891,53.839,49.372Q53.683,49.853,53.683,50.49Q53.683,51.127,53.839,51.608000000000004Q53.995000000000005,52.089,54.3493,52.3555Q54.7035,52.622,55.295,52.622ZM62.978,54.169Q62.275999999999996,54.169,61.638999999999996,53.8862Q61.001999999999995,53.6035,60.5308,53.09Q60.0595,52.576499999999996,59.858000000000004,51.881L61.574,51.426Q61.710499999999996,51.9395,62.110299999999995,52.2222Q62.510000000000005,52.505,62.978,52.505Q63.381,52.505,63.7158,52.31Q64.0505,52.115,64.2488,51.783500000000004Q64.447,51.452,64.447,51.049Q64.447,50.4445,64.0343,50.0122Q63.6215,49.58,62.978,49.58Q62.783,49.58,62.601,49.63525Q62.419,49.6905,62.25,49.788L61.457,48.397L64.434,45.927L64.564,46.304L60.222,46.304L60.222,44.64L66.072,44.64L66.072,46.304L63.757999999999996,48.54L63.745000000000005,48.046Q64.551,48.1695,65.10679999999999,48.60825Q65.6625,49.047,65.95179999999999,49.68725Q66.241,50.3275,66.241,51.049Q66.241,51.933,65.79249999999999,52.6383Q65.344,53.3435,64.60300000000001,53.756299999999996Q63.861999999999995,54.169,62.978,54.169Z" fill="#AD44FF"></path>
                                </svg>
                            </div>
                        </div>
                    </div>
                </div>
                <div className="other-products">
                    <div className="other-products-title">Chain Abstraction</div>
                    <div className="other-products-list">
                        <a className="other-products-link" target="_blank" href="https://developers.particle.network/docs/particle-chain">
                            <div>Modular L1</div>
                        </a>
                        <div className="dot"></div>
                        <a className="other-products-link" target="_blank" href="https://developers.particle.network/docs/universal-accounts">
                            <div>Universal Accounts</div>
                        </a>
                        <div className="dot"></div>
                        <a className="other-products-link" target="_blank" href="https://developers.particle.network/docs/universal-liquidity">
                            <div>Universal Liquidity</div>
                        </a>
                        <div className="dot"></div>
                        <a className="other-products-link" target="_blank" href="https://developers.particle.network/docs/universal-gas">
                            <div>Universal Gas</div>
                        </a>
                    </div>
                </div>
                <div className="chains">
                    <div className="halo-middle-left"></div>
                    <img className="animation-chains" src="https://files.readme.io/322a71b-20240124-195115.png" />
                    <img className="animation-background" src="https://files.readme.io/029d834-20240125-150108.png" />
                </div>
                <div className="sponsors">
                    <div className="halo-bottom-left"></div>
                    <div className="halo-bottom-right"></div>
                    <div className="sponsors-title">Trusted by the best in Web3</div>
                    <div className="sponsors-img">
                        <img src="https://files.readme.io/e5f2b48-sponsors2.png" />
                    </div>
                </div>
                <div className="plug">
                    <div className="plug-logo">
                        <img src="https://static.particle.network/docs-images/logo.png" />
                    </div>
                    <div className="animation-text">
                        <img src="https://files.readme.io/819a28e-20240126-191004.png" />
                    </div>
                </div>
                <footer className="footer-container">
                    <div className="wrapper">
                        <div className="row row-1">
                            <div className="col col-1">
                                <div className="logo">
                                    <img src="https://static.particle.network/docs-images/footer_logo.png" alt="logo" />
                                </div>
                                <div className="icons">
                                    <a target="_blank" href="https://twitter.com/ParticleNtwrk">
                                        <img src="https://static.particle.network/docs-images/twitter.png" />
                                    </a>
                                    <a target="_blank" href="https://discord.com/invite/2y44qr6CR2">
                                        <img src="https://static.particle.network/docs-images/discord.png" />
                                    </a>
                                    <a target="_blank" href="https://blog.particle.network/">
                                        <img src="https://files.readme.io/b1160af-_12550.png" />
                                    </a>
                                </div>
                                <div className="copy-write">
                                    <span>© 2024 PARTICLE NETWORK. ALL RIGHTS RESERVED</span>
                                </div>
                            </div>
                            <div className="col col-2">
                                <div className="title">Products</div>
                                <div className="list">
                                    <div className="item">
                                        <a href="https://particle.network/modular-smart-waas.html" target="_blank">Modular Smart WaaS</a>
                                    </div>
                                    <div className="item">
                                        <a href="https://particle.network/confidential-zkstack.html" target="_blank">Confidential zkStack</a>
                                    </div>
                                    <div className="item">
                                        <a href="https://particle.network/intent-fusion-protocol.html" target="_blank">Intent Fusion Protocol</a>
                                    </div>
                                    <div className="item item-aa">
                                        <a href="https://particle.network/omnichain-aa.html" target="_blank">
                                            Omnichain Account Abstraction
                                        </a>
                                    </div>
                                    <div className="item item-aa-mobile">
                                        <a href="https://particle.network/omnichain-aa.html" target="_blank">
                                            Omnichain AA
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a href="https://particle.network/unified-gas-token.html" target="_blank">Unified Gas Token</a>
                                    </div>
                                    <div className="item">
                                        <a href="https://particle.network/btc-connect.html" target="_blank">BTC Connect</a>
                                    </div>
                                </div>
                            </div>
                            <div className="col col-3">
                                <div className="title">Developers</div>
                                <div className="list">
                                    <div className="item">
                                        <a target="_blank" href="https://dashboard.particle.network">
                                            Dashboard
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://github.com/Particle-Network">
                                            Github
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://docs.particle.network/">
                                            Docs
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://docs.particle.network/overview/security">
                                            Security
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://discord.com/invite/2y44qr6CR2">
                                            Community
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <div className="col col-4">
                                <div className="title">Company</div>
                                <div className="list">
                                    <div className="item">
                                        <a target="_blank" href="https://blog.particle.network/">
                                            Blog
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://www.linkedin.com/company/particlenetwork">
                                            LinkedIn
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://discord.com/invite/2y44qr6CR2">
                                            Discord
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://calendly.com/particle-network/30min">
                                            Schedule Demo
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <div className="col col-4">
                                <div className="title">Legal</div>
                                <div className="list">
                                    <div className="item">
                                        <a target="_blank" href="https://docs.particle.network/resources/terms-and-conditions/terms-of-use">
                                            Term of use
                                        </a>
                                    </div>
                                    <div className="item">
                                        <a target="_blank" href="https://docs.particle.network/resources/terms-and-conditions/privacy-policy">
                                            Privacy Policy
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div className="row row-3">
                            <div className="footer-icon">
                                <div className="img">
                                    <img src="https://static.particle.network/docs-images/footer_icon.png" />
                                </div>
                                <div className="bg-content">
                                    <div className="wrap">
                                        <img id="footer-img" src="https://static.particle.network/docs-images/footer_background.png" />
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </footer>
            </div>
        </>
    );
}

```