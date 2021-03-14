# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Appia - Angular 11 App Landing Page` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'appia';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { HeroOneComponent } from './components/hero/hero-one/hero-one.component';
import { HeroTwoComponent } from './components/hero/hero-two/hero-two.component';
import { HeroThreeComponent } from './components/hero/hero-three/hero-three.component';
import { HeroFourComponent } from './components/hero/hero-four/hero-four.component';
import { HeroFiveComponent } from './components/hero/hero-five/hero-five.component';
import { HeroSixComponent } from './components/hero/hero-six/hero-six.component';
import { PromoOneComponent } from './components/promo/promo-one/promo-one.component';
import { PromoTwoComponent } from './components/promo/promo-two/promo-two.component';
import { PromoThreeComponent } from './components/promo/promo-three/promo-three.component';
import { PromoFourComponent } from './components/promo/promo-four/promo-four.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { FeatureOneComponent } from './components/features/feature-one/feature-one.component';
import { FeatureTwoComponent } from './components/features/feature-two/feature-two.component';
import { FeatureThreeComponent } from './components/features/feature-three/feature-three.component';
import { ScreenshotOneComponent } from './components/screenshots/screenshot-one/screenshot-one.component';
import { ScreenshotTwoComponent } from './components/screenshots/screenshot-two/screenshot-two.component';
import { ContentOneComponent } from './components/content/content-one/content-one.component';
import { ContentTwoComponent } from './components/content/content-two/content-two.component';
import { ContentThreeComponent } from './components/content/content-three/content-three.component';
import { ContentFourComponent } from './components/content/content-four/content-four.component';
import { ContentFiveComponent } from './components/content/content-five/content-five.component';
import { ContentSixComponent } from './components/content/content-six/content-six.component';
import { ContentSevenComponent } from './components/content/content-seven/content-seven.component';
import { ContentEightComponent } from './components/content/content-eight/content-eight.component';
import { ContentNineComponent } from './components/content/content-nine/content-nine.component';
import { PricingOneComponent } from './components/pricing/pricing-one/pricing-one.component';
import { PricingTwoComponent } from './components/pricing/pricing-two/pricing-two.component';
import { PricingThreeComponent } from './components/pricing/pricing-three/pricing-three.component';
import { ReviewComponent } from './components/review/review.component';
import { TeamOneComponent } from './components/team/team-one/team-one.component';
import { TeamTwoComponent } from './components/team/team-two/team-two.component';
import { CtaOneComponent } from './components/cta/cta-one/cta-one.component';
import { CtaTwoComponent } from './components/cta/cta-two/cta-two.component';
import { DownloadOneComponent } from './components/download/download-one/download-one.component';
import { DownloadTwoComponent } from './components/download/download-two/download-two.component';
import { FaqOneComponent } from './components/faq/faq-one/faq-one.component';
import { FaqTwoComponent } from './components/faq/faq-two/faq-two.component';
import { ContactComponent } from './components/contact/contact.component';
import { FooterOneComponent } from './components/footer/footer-one/footer-one.component';
import { FooterTwoComponent } from './components/footer/footer-two/footer-two.component';
import { FooterThreeComponent } from './components/footer/footer-three/footer-three.component';
import { FooterFourComponent } from './components/footer/footer-four/footer-four.component';
import { FooterFiveComponent } from './components/footer/footer-five/footer-five.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { HeaderOneComponent } from './components/header/header-one/header-one.component';
import { HeaderTwoComponent } from './components/header/header-two/header-two.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { VideoComponent } from './components/video/video.component';
import { AboutOneComponent } from './components/about/about-one/about-one.component';
import { AboutTwoComponent } from './components/about/about-two/about-two.component';
import { CounterOneComponent } from './components/counter/counter-one/counter-one.component';
import { CounterTwoComponent } from './components/counter/counter-two/counter-two.component';
import { BrandingComponent } from './components/branding/branding.component';
import { BreadcrumbOneComponent } from './components/breadcrumb/breadcrumb-one/breadcrumb-one.component';
import { BreadcrumbTwoComponent } from './components/breadcrumb/breadcrumb-two/breadcrumb-two.component';
import { BreadcrumbThreeComponent } from './components/breadcrumb/breadcrumb-three/breadcrumb-three.component';
import { BreadcrumbFourComponent } from './components/breadcrumb/breadcrumb-four/breadcrumb-four.component';
import { BreadcrumbFiveComponent } from './components/breadcrumb/breadcrumb-five/breadcrumb-five.component';
import { BreadcrumbSixComponent } from './components/breadcrumb/breadcrumb-six/breadcrumb-six.component';
import { BreadcrumbSevenComponent } from './components/breadcrumb/breadcrumb-seven/breadcrumb-seven.component';
import { BreadcrumbEightComponent } from './components/breadcrumb/breadcrumb-eight/breadcrumb-eight.component';
import { BreadcrumbNineComponent } from './components/breadcrumb/breadcrumb-nine/breadcrumb-nine.component';
import { BreadcrumbTenComponent } from './components/breadcrumb/breadcrumb-ten/breadcrumb-ten.component';
import { FooterSixComponent } from './components/footer/footer-six/footer-six.component';
import { MapComponent } from './components/map/map.component';
import { BlogOneComponent } from './components/blog/blog-one/blog-one.component';
import { BlogTwoComponent } from './components/blog/blog-two/blog-two.component';
import { BlogThreeComponent } from './components/blog/blog-three/blog-three.component';
import { BlogFourComponent } from './components/blog/blog-four/blog-four.component';
import { BlogFiveComponent } from './components/blog/blog-five/blog-five.component';
import { BlogSixComponent } from './components/blog/blog-six/blog-six.component';
import { PricingPageComponent } from './components/inner-pages/pricing-page/pricing-page.component';
import { ReviewPageComponent } from './components/inner-pages/review-page/review-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { NewsletterComponent } from './components/inner-pages/newsletter/newsletter.component';
import { ErrorOneComponent } from './components/inner-pages/error-page/error-one/error-one.component';
import { ErrorTwoComponent } from './components/inner-pages/error-page/error-two/error-two.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { MaintenanceComponent } from './components/inner-pages/maintenance/maintenance.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { BlogTwoColumnComponent } from './components/inner-pages/blog-page/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/inner-pages/blog-page/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/inner-pages/blog-page/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/inner-pages/blog-page/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/inner-pages/blog-page/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/inner-pages/blog-page/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { LoginComponent } from './components/inner-pages/accounts/login/login.component';
import { SignupComponent } from './components/inner-pages/accounts/signup/signup.component';
import { ForgotComponent } from './components/inner-pages/accounts/forgot/forgot.component';
import { FaqThreeComponent } from './components/faq/faq-three/faq-three.component';

@NgModule({
  declarations: [
    AppComponent,
    HeroOneComponent,
    HeroTwoComponent,
    HeroThreeComponent,
    HeroFourComponent,
    HeroFiveComponent,
    HeroSixComponent,
    PromoOneComponent,
    PromoTwoComponent,
    PromoThreeComponent,
    PromoFourComponent,
    ThemeOneComponent,
    FeatureOneComponent,
    FeatureTwoComponent,
    FeatureThreeComponent,
    ScreenshotOneComponent,
    ScreenshotTwoComponent,
    ContentOneComponent,
    ContentTwoComponent,
    ContentThreeComponent,
    ContentFourComponent,
    ContentFiveComponent,
    ContentSixComponent,
    ContentSevenComponent,
    ContentEightComponent,
    ContentNineComponent,
    PricingOneComponent,
    PricingTwoComponent,
    PricingThreeComponent,
    ReviewComponent,
    TeamOneComponent,
    TeamTwoComponent,
    CtaOneComponent,
    CtaTwoComponent,
    DownloadOneComponent,
    DownloadTwoComponent,
    FaqOneComponent,
    FaqTwoComponent,
    ContactComponent,
    FooterOneComponent,
    FooterTwoComponent,
    FooterThreeComponent,
    FooterFourComponent,
    FooterFiveComponent,
    ScrollupComponent,
    HeaderOneComponent,
    HeaderTwoComponent,
    ThemeTwoComponent,
    ThemeThreeComponent,
    ThemeFourComponent,
    ThemeFiveComponent,
    ThemeSixComponent,
    VideoComponent,
    AboutOneComponent,
    AboutTwoComponent,
    CounterOneComponent,
    CounterTwoComponent,
    BrandingComponent,
    BreadcrumbOneComponent,
    BreadcrumbTwoComponent,
    BreadcrumbThreeComponent,
    BreadcrumbFourComponent,
    BreadcrumbFiveComponent,
    BreadcrumbSixComponent,
    BreadcrumbSevenComponent,
    BreadcrumbEightComponent,
    BreadcrumbNineComponent,
    BreadcrumbTenComponent,
    FooterSixComponent,
    MapComponent,
    BlogOneComponent,
    BlogTwoComponent,
    BlogThreeComponent,
    BlogFourComponent,
    BlogFiveComponent,
    BlogSixComponent,
    PricingPageComponent,
    ReviewPageComponent,
    FaqPageComponent,
    DownloadPageComponent,
    ThankYouComponent,
    NewsletterComponent,
    ErrorOneComponent,
    ErrorTwoComponent,
    ContactPageComponent,
    MaintenanceComponent,
    ComingSoonComponent,
    BlogTwoColumnComponent,
    BlogThreeColumnComponent,
    BlogLeftSidebarComponent,
    BlogRightSidebarComponent,
    BlogDetailsLeftSidebarComponent,
    BlogDetailsRightSidebarComponent,
    LoginComponent,
    SignupComponent,
    ForgotComponent,
    FaqThreeComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- theme-two ( demo theme 2)
    .....
    |-- theme-six ( demo theme 6 )
```

`themes` folder contains all of our 6 page demos.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';

import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { PricingPageComponent } from './components/inner-pages/pricing-page/pricing-page.component';
import { ReviewPageComponent } from './components/inner-pages/review-page/review-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { LoginComponent } from './components/inner-pages/accounts/login/login.component';
import { SignupComponent } from './components/inner-pages/accounts/signup/signup.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { ForgotComponent } from './components/inner-pages/accounts/forgot/forgot.component';
import { NewsletterComponent } from './components/inner-pages/newsletter/newsletter.component';
import { ErrorOneComponent } from './components/inner-pages/error-page/error-one/error-one.component';
import { ErrorTwoComponent } from './components/inner-pages/error-page/error-two/error-two.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { MaintenanceComponent } from './components/inner-pages/maintenance/maintenance.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { BlogTwoColumnComponent } from './components/inner-pages/blog-page/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/inner-pages/blog-page/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/inner-pages/blog-page/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/inner-pages/blog-page/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/inner-pages/blog-page/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/inner-pages/blog-page/blog-details-right-sidebar/blog-details-right-sidebar.component';


const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'theme-two', component: ThemeTwoComponent},
  {path: 'theme-three', component: ThemeThreeComponent},
  {path: 'theme-four', component: ThemeFourComponent},
  {path: 'theme-five', component: ThemeFiveComponent},
  {path: 'theme-six', component: ThemeSixComponent},
  {path: 'pricing', component: PricingPageComponent},
  {path: 'reviews', component: ReviewPageComponent},
  {path: 'faq', component: FaqPageComponent},
  {path: 'login', component: LoginComponent},
  {path: 'signup', component: SignupComponent},
  {path: 'download', component: DownloadPageComponent},
  {path: 'thank-you', component: ThankYouComponent},
  {path: 'forgot', component: ForgotComponent},
  {path: 'newsletter', component: NewsletterComponent},
  {path: 'error-one', component: ErrorOneComponent},
  {path: 'error-two', component: ErrorTwoComponent},
  {path: 'contact', component: ContactPageComponent},
  {path: 'maintenance', component: MaintenanceComponent},
  {path: 'coming-soon', component: ComingSoonComponent},
  {path: 'blog-two-column', component: BlogTwoColumnComponent},
  {path: 'blog-three-column', component: BlogThreeColumnComponent},
  {path: 'blog-left-sidebar', component: BlogLeftSidebarComponent},
  {path: 'blog-right-sidebar', component: BlogRightSidebarComponent},
  {path: 'blog-details-left-sidebar', component: BlogDetailsLeftSidebarComponent},
  {path: 'blog-details-right-sidebar', component: BlogDetailsRightSidebarComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `hero` , `footer` folder where we wrote our different styled component. For example `hero` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- hero ( hero component folder )
        - hero-one ( main demo hero section )
        - hero-two ( demo two hero section )
        ...... ( and other )
    ...    
```

### Contact Page component
`inner-pages/contact-page/contact-page.component.html`

```text
|-- components
    ....
    ..
    |-- inner-pages ( all inner-pages folder )
        ......
        - contact-page ( contact-page component )
        ...... ( and other )
    ...    
```

```html
<div class="inner">
    <app-scrollup></app-scrollup>
    <div class="main">
        <app-header-two></app-header-two>
        <app-breadcrumb-four></app-breadcrumb-four>
        <app-contact></app-contact>
        <app-map></app-map>
        <app-footer-six></app-footer-six>
    </div>
</div>
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
