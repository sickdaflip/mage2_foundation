# Create CMS_Blocks for this Theme

------------

#### Header Top Promo Bar > header-top-bar

    Comming soon: Black Week 20XX!

#### Header Contact & Links > header-contact-links

    <div class="contact-bar__container" data-content-type="html" data-appearance="default" data-element="main">
      <ul class="list contact-bar__list">
        <li class="list-item contact-bar__item">
          <a class="contact-bar__link" href="{{store url="customer/account"}}">
            <span class="button__text contact-bar__text">Account</span>
          </a>
        </li>
        <li class="list-item contact-bar__item">
          <a class="contact-bar__link" href="{{store url="contact"}}">
            <span class="button__text contact-bar__text">Kontakt</span>
          </a>
        </li>
      </ul>
      <ul class="list contact-bar__list contact-bar__list--icons">
        <li class="list-item contact-bar__item">
          <a class="contact-bar__link" href="tel:+498001234567">
            <span class="contact-bar__icon" aria-label="">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="phone" title="Phone"}}
            </span>
            <span class="contact-bar__text">Hotline +49 (0)800 - 123 - 4567</span>
          </a>
        </li>
        <li class="contact-bar__item">
          <a class="contact-bar__link" href="mailto:johndoe@universe.com">
            <span class="contact-bar__icon" aria-label="">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="envelope" title="Email"}}
            </span>
            <span class="contact-bar__text">Email</span>
          </a>
        </li>
        <li class="list-item contact-bar__item">
          <a class="contact-bar__link">
            <span class="contact-bar__icon" aria-label="">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="delivery-truck" title="Delivery"}}
            </span>
            <span class="contact-bar__text">fast &amp; cheap shipping</span>
          </a>
        </li>
        <li class="list-item contact-bar__item">
          <a class="contact-bar__link">
            <span class="contact-bar__icon" aria-label="">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="thumb-up" title="Customers"}}
            </span>
            <span class="contact-bar__text">over 100.000 satisfied costumers</span>
          </a>
        </li>
      </ul>
    </div>

#### Header Brief Info > header-brief-info

    <div class="brief-info">
      <ul class="list brief-info__items-container">
        <li class="brief-info__item">
          <span class="brief-info__icon-wrapper margin-right-xs" aria-label="Quality">
            {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="shield" title="Quality" icon_class="brief-info__icon" role="presentation"}}
          </span>
          <div class="brief-info__content">
            <p class="brief-info__title ">Quality</p>
            <p class="brief-info__subtitle">since 2000</p>
          </div>
        </li>
        <li class="brief-info__item">
          <span class="brief-info__icon-wrapper margin-right-xs" aria-label="Free shipping">
            {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="delivery-truck" title="Free shipping" icon_class="brief-info__icon" role="presentation"}}
          </span>
          <div class="brief-info__content">
            <p class="brief-info__title ">free shipping</p>
            <p class="brief-info__subtitle">from 99 EUR</p>
          </div>
        </li>
      </ul>
    </div>

#### Footer Newsletter > footer-newsletter

    <h2 class="newsletter__title">Join our email list</h2>
    <p class="newsletter__subtitle">Sign up for savings and product announcements</p>

#### Footer Newsletter Terms > footer-newsletter-terms

    <span class="checkbox__text">I agree to <a title="Terms and conditions" href="/terms-conditions">Terms and conditions</a> and I am happy to receive your newsletter with all your promotions.</span>

#### Footer Social > footer-social

    <div class="footer__social-handler" data-content-type="html" data-appearance="default" data-element="main">
      <h3 class="footer__social-list-title">Let's get social!</h3>
      <ul class="list list--with-icon list--horizontal footer__social-list">
        <li class="list__item">
          <a class="list__icon-link button button--icon button--icon-border" href="#" aria-label="Go to Our Facebook Page">
            {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="facebook" title="Facebook logo" icon_class="icon footer__social-icon"}}
          </a>
        </li>
        <li class="list__item">
          <a class="list__icon-link button button--icon button--icon-border" href="#" aria-label="Check our Twitter">
            {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="twitter" title="Twitter logo" icon_class="icon footer__social-icon"}}
          </a>
        </li>
      </ul>
    </div>

#### Footer Bottom Bar > footer-bottom-bar

    <div class="footer__copyright">
      <small>Copyright © 2023 JohnDoe</small>
    </div>
    <ul class="footer__payments-list list list--horizontal">
      <li class="list__item">
        {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="visa" title="Visa" icon_class="footer__payments-list-icon footer__payments-list-icon--visa"}}
      </li>
      <li class="list__item">
        {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="master-card" title="Master Card" icon_class="footer__payments-list-icon"}}
      </li>
      <li class="list__item">
        {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="discover" title="Discover" icon_class="footer__payments-list-icon"}}
      </li>
      <li class="list__item">
        {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="american-express" title="American Express" icon_class="footer__payments-list-icon"}}
      </li>
      <li class="list__item">
        {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="paypal" title="PayPal" icon_class="footer__payments-list-icon"}}
      </li>
    </ul>

#### Footer Cookie Message > footer-cookie-message
- (optional) better use consent-plugin


    <p class="cookie-message__text">Find out more about their purpose and settings in your browser. By browsing the site you are agreeing to use cookies according to your browser settings.
        <a title="Privacy and Cookie Policy" href="privacy-policy-cookie-restriction-mode" target="_blank" rel="noopener">Privacy and Cookie Policy
        </a>
    </p>

#### Contact form description > contact-form-description

    <p>Jot us a note and we’ll get back to you as quickly as possible.</p>

#### Home brief info > home-brief-info

    <section class="section display-none-m">
      <div class="section__content">
        <div class="brief-info brief-info--dividers">
          <ul class="list brief-info__items-container">
            <li class="brief-info__item">
              <span class="brief-info__icon-wrapper margin-right-xs" aria-label="Return policy">
                {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="return" icon_class="icon brief-info__icon" title="Return Policy" role="presentation"}}
              </span>
              <div class="brief-info__content">
                <h3 class="brief-info__title">Lorem Ipsum is simply</h3>
                <p class="brief-info__subtitle">30-day return policy</p>
              </div>
            </li>
            <li class="brief-info__item">
              <span class="brief-info__icon-wrapper margin-right-xs" aria-label="Lorem Ipsum is simply">
                {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="bigstar" icon_class="icon brief-info__icon" title="Big star" role="presentation"}}
              </span>
              <div class="brief-info__content">
                <h3 class="brief-info__title">Lorem Ipsum is simply</h3>
                <p class="brief-info__subtitle">Now in stock!</p>
              </div>
            </li>
            <li class="brief-info__item">
              <span class="brief-info__icon-wrapper margin-right-xs" aria-label="Our Customers Are Talking">
                {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="reviews" icon_class="icon brief-info__icon" title="Our Customers Are Talking" role="presentation"}}
              </span>
              <div class="brief-info__content">
                <h3 class="brief-info__title ">Our Customers Are Talking</h3>
                <p class="brief-info__subtitle">Check out our reviews!</p>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </section>

#### Home categories banners > home-categories-banners

    <section class="section section--fix-spacer-large">
      <header class="section__heading">
        <h2 class="heading--first-level margin-0">Shop by category</h2>
      </header>
      <div class="section__content row">
        <a class="banner col-xs-6 col-lg-3 home__category-banner margin-bottom-l" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
          img480="wysiwyg/home/blabla_480.jpg"
          img_full="wysiwyg/home/blabla_1024.jpg"
          picture_class="image"
          picture_alt="banner alt"
          img_ratio_width="400"
          img_ratio_height="400"
          id="category-home-banner-1" }}
          <span class="banner__content">
            <span class="banner__text">Test</span>
            <span class="banner__icon">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="arrow-right" icon_class="" title="Arrow right icon" role="presentation"}}
            </span>
          </span>
        </a>
        <a class="banner col-xs-6 col-lg-3 home__category-banner margin-bottom-l" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
          img480="wysiwyg/home/blabla_480.jpg"
          img_full="wysiwyg/home/blabla_1024.jpg"
          picture_class="image"
          picture_alt="banner alt"
          img_ratio_width="400"
          img_ratio_height="400"
          id="category-home-banner-1" }}
          <span class="banner__content">
            <span class="banner__text">Test</span>
            <span class="banner__icon">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="arrow-right" icon_class="" title="Arrow right icon" role="presentation"}}
            </span>
          </span>
        </a>
        <a class="banner col-xs-6 col-lg-3 home__category-banner margin-bottom-l" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
          img480="wysiwyg/home/blabla_480.jpg"
          img_full="wysiwyg/home/blabla_1024.jpg"
          picture_class="image"
          picture_alt="banner alt"
          img_ratio_width="400"
          img_ratio_height="400"
          id="category-home-banner-1" }}
          <span class="banner__content">
            <span class="banner__text">Test</span>
            <span class="banner__icon">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="arrow-right" icon_class="" title="Arrow right icon" role="presentation"}}
            </span>
          </span>
        </a>
        <a class="banner col-xs-6 col-lg-3 home__category-banner margin-bottom-l" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
          img480="wysiwyg/home/blabla_480.jpg"
          img_full="wysiwyg/home/blabla_1024.jpg"
          picture_class="image"
          picture_alt="banner alt"
          img_ratio_width="400"
          img_ratio_height="400"
          id="category-home-banner-1" }}
          <span class="banner__content">
            <span class="banner__text">Test</span>
            <span class="banner__icon">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="arrow-right" icon_class="" title="Arrow right icon" role="presentation"}}
            </span>
          </span>
        </a>
      </div>
    </section>

#### Home additional banners > home-additional-banners

    <section class="section section--fix-spacer-medium">
      <div class="section__content row">
        <a class="banner col-xs-12 col-lg-6 home__banner" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
            img_default="wysiwyg/home/blabla_1024.jpg"
            picture_class="image"
            picture_alt="banner alt"
            img_ratio_width="1920"
            img_ratio_height="425" }}
        </a>
        <a class="banner col-xs-12 col-lg-6 home__banner" href="{{store url="#"}}" aria-label="descriptive text about banner action and / or image">
          {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
            img_default="wysiwyg/home/blabla_1024.jpg"
            picture_class="image"
            picture_alt="banner alt"
            img_ratio_width="1920"
            img_ratio_height="425" }}
        </a>
      </div>
    </section>

#### Home products widget > home-products-widget

    <section class="section">
        {{widget type="Magento\CatalogWidget\Block\Product\ProductsList" title="Bestsellers" show_pager="0" products_count="10" template="Magento_CatalogWidget::product/widget/content/grid.phtml" conditions_encoded="^[`1`:^[`type`:`Smile||ElasticsuiteVirtualCategory||Model||Rule||WidgetCondition||Combine`,`aggregator`:`any`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Smile||ElasticsuiteVirtualCategory||Model||Rule||WidgetCondition||Product`,`attribute`:`sku`,`operator`:`^[^]`,`value`:`24-MB01, 24-MB04, 24-MB03, 24-MB05, 24-MB06, 24-MB02, 24-UB02, 24-WB01, 24-WB02, 24-WB05, 24-WB06, 24-WB03, 24-WB07, 24-WB04, 24-UG06, 24-UG07, 24-UG04, 24-UG02, 24-UG05, 24-UG01`^]^]"}}
    </section>

#### Home NEW products widget > home-new-products-widget

    <section class="section">
        {{widget type="Magento\CatalogWidget\Block\Product\ProductsList" title="New products" show_pager="0" products_count="10" template="Magento_CatalogWidget::product/widget/content/grid.phtml" conditions_encoded="^[`1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Combine`,`aggregator`:`any`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Product`,`attribute`:`sku`,`operator`:`()`,`value`:`24-MB01, 24-MB04, 24-MB03, 24-MB05, 24-MB06, 24-MB02, 24-UB02, 24-WB01, 24-WB02, 24-WB05, 24-WB06, 24-WB03, 24-WB07, 24-WB04, 24-UG06, 24-UG07, 24-UG04, 24-UG02, 24-UG05, 24-UG01`^]^]"}}
    </section>

#### Home Slider > home-slider

    {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/slider.phtml" sliderHtml="before-slides" dots="no" arrows="yes"}}
    <div class="slider__item">
      {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
      id="Investrabatt"
      picture_class="picture"
      lazy="true"
      mediaUrl="true"
      img_default="wysiwyg/home/blabla_1024.jpg"
      img480="wysiwyg/home/blabla_480.jpg"}}
    </div>
    <div class="slider__item">
      {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
      id="Investrabatt"
      picture_class="picture"
      lazy="true"
      mediaUrl="true"
      img_default="wysiwyg/home/blabla_1024.jpg"
      img480="wysiwyg/home/blabla_480.jpg"}}
    </div>
    <div class="slider__item">
      {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
      id="Investrabatt"
      picture_class="picture"
      lazy="true"
      mediaUrl="true"
      img_default="wysiwyg/home/blabla_1024.jpg"
      img480="wysiwyg/home/blabla_480.jpg"}}
    </div>
    {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/slider.phtml" sliderHtml="after-slides"}}

#### Home teasers > home-teasers

    <div data-content-type="html" data-appearance="default" data-element="main">
      <section class="section">
        <div class="section__content">
          <div class="teaser teaser--secondary">
            <div class="teaser__image">
              {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/picture.phtml"
              img_full="wysiwyg/home/blabla_1024.jpg"
              picture_alt="teaser alt"
              img_ratio_width="1024"
              img_ratio_height="1024"
              id="home-teaser-picture"}}
            </div>
            <div class="teaser__content">
              <div class="teaser__content-block">
                <div class="content-block">
                  <div class="row">
                    <div class="col-xs-12">
                      <h2 class="content-block__heading">Lorem ipsum</h2>
                      <div class="paragraph content-block__description">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text</div>
                      <a class="link content-block__link" title="Title" href="{{store url="#"}}">Read more</a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>

#### Home content > home-content

    <section class="section">
      <div class="section__content">
        <div class="content-block content-block--secondary">
          <div class="content-block__row row between-lg evenly-xl">
            <div class="content-block__column col-xs-12 col-lg-4 col-xl-3">
              <h2 class="heading--first-level content-block__heading  content-block__heading--secondary">Lorem ipsum is simply</h2>
            </div>
            <div class="content-block__column col-xs-12 col-lg-7 col-xl-6">
              <div class="paragraph content-block__introduction">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s</div>
              <div class="paragraph content-block__description">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris, Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris</div>
            </div>
          </div>
        </div>
      </div>
    </section>

#### Catalog Search - no results > search-no-results

    <p><strong>We can't find products matching the selection.</strong></p>
    <p><br>Try again selecting other criteria</p>
    <p><br>or</p>

#### Privacy FAQs > prgdpr_privacy_faqs
-(optional) better use consent-plugin


    <div class="prgdpr__faq">
      <h2 class="prgdpr__title">Privacy FAQs</h2>
      <p class="prgdpr__descr">Learn how our policies put transparency, simplicity, and control into action for you.</p>
      <ul class="prgdpr-accordion">
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">What information do you collect about me?</b>
          <div class="prgdpr-accordion__descr">
            <p>Initially, we collect basic information from you to create your account, including your full name, email and password. We collect further data, such as address, and billing information or other information you provide when you checkout at our store. We also collect some information about users who visit our websites using cookies and similar technologies. See the Privacy Policy and/or Cookie Policy for the particular website(s) or service(s) you are using for more details about the specific types of information we may collect and your choices related to that data.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">How do you use information about me?</b>
          <div class="prgdpr-accordion__descr">
            <p>We primarily use information about you to provide, personalize, improve, update and expand and improve our services to you. For example, we use information about you to create your account and deliver our products and services. We may also use your information to improve or develop new products and services, and for internal business purposes. We may also use personal information about you to verify your identity, communicate with you and to deliver advertisements, issuing surveys and questionnaires to collect additional user information for use in the services, marketing new products and offers from us or our business partners, detecting and protecting against error, fraud, or other criminal or malicious activity. See our Privacy Policy for more details.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">Do you share information about me?</b>
          <div class="prgdpr-accordion__descr">
            <p>We do not share your personal information with third-parties without your additional consent other than as described in our Privacy Policy. Otherwise, we share information as described in our Privacy Policy, such as with our affiliated companies, our service providers, our advertising partners, and in other limited scenarios, such as in response to valid legal process or as appropriate to protect the rights, property, safety, confidentiality, or reputation of our company, our affiliates, and our users. You can read the Privacy Policy for the particular website(s) or service(s) you are using for more details about how we share your data and your choices related to that sharing.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">How can I review, update, or delete information about me?</b>
          <div class="prgdpr-accordion__descr">
            <p>You can review, update, or delete most information about yourself through your account page on our website. If you have questions about how to review, update, or delete information, you should contact our Data Protection Office or Customer Services team.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">What happens to my information if I delete my account?</b>
          <div class="prgdpr-accordion__descr">
            <p>When you delete your account, we remove your information from our store (it may take up to 30 days to make sure everything is deleted). During that period, you won't be able to use your account. Our company also retains certain data to comply with local laws, such as sales receipts to comply with local tax laws.</p>
            <p>Please keep in mind that once your account has been deleted you won't be able to reactivate your account or retrieve anything you've added, including:</p>
            <ul>
              <li>Your billing information</li>
              <li>Your orders, invoices, shipments</li>
              <li>Any history of interactions with our support</li>
              <li>Any content you have created associated with your store account</li>
              <li>You also will no longer be able to return any products or services and will lose any existing store rewards or credits</li>
            </ul>
            <p>If you decide that you no longer wish to delete your store account, you can cancel your deletion request within 24 hours of making the deletion request by login in to your account.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">What are you doing to protect my personal information?</b>
          <div class="prgdpr-accordion__descr">
            <p>We work hard to protect our customers from unauthorized access, use and disclosure of information. We store and process the information we collect on computer systems with limited access, which are located in controlled facilities. Any sensitive information is protected through the use of best-practice physical, environmental and digital security systems.</p>
          </div>
        </li>
        <li class="prgdpr-accordion__item">
          <input class="prgdpr-accordion__toggle" checked="checked" type="checkbox" />
          <i class="prgdpr-accordion__btn"></i>
          <b class="prgdpr__name prgdpr-accordion__name">What can I do to protect my personal information?</b>
          <div class="prgdpr-accordion__descr">
            <p>There are a number of measures that you can take to protect your personal information, including:</p>
            <ul>
              <li>Use strong passwords for all your online accounts</li>
              <li>Do keep passwords securely (never written down, or shared with anyone) and changed periodically</li>
              <li>Don't automatically trust every website or email which asks you to provide your personal information. Take time to check that the request is valid, and that the personal information requested is absolutely necessary for the services that you are looking to use</li>
            </ul>
          </div>
        </li>
      </ul>
    </div>
    <div class="prgdpr__footer">
      <p class="prgdpr__footer-text-top">Please contact our Data Protection Officer with any questions or concerns via email at <a href="mailto:privacy@domain.com">privacy@domain.com</a> or via postal mail at:</p>
      <p class="prgdpr__address">Data Protection Officer<br /> Your Company<br /> 123 Street, Suite 444<br /> New York, NY 10001<br /> USA</p>
    </div>

#### Popup product button benefit 1 > popup-product-button-benefit-1

    <div class="brief-info__icon-wrapper margin-right-xs" aria-label="Delivery">
      {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="delivery-truck" title="Free shipping icon" icon_class="icon brief-info__icon" role="presentation" focusable="false"}}
    </div>
    <div class="brief-info__content">
      <h3 class="brief-info__title">Free Shipping</h3>
      <p class="brief-info__subtitle">On Hundreds of Products</p>
    </div>

#### Popup product benefit 1 > popup-product-benefit-1

    <h2>Popup Product Benefit 1!</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel dui at dui rhoncus molestie. Praesent imperdiet semper gravida. Fusce ultricies dapibus magna, a fermentum purus viverra sed.</p>
    <p>Cras sed ultricies enim. Sed suscipit quis neque a porttitor. Phasellus aliquam ex ac mattis tincidunt. Lorem ipsum dolor sit amet, c</p>

#### Popup product button benefit 2 > popup-product-button-benefit-2

    <div class="brief-info__icon-wrapper margin-right-xs" aria-label="Return Policy">
      {{block class="Magento\Framework\View\Element\Template" template="Magento_Theme::html/svg-icon.phtml" icon="return" title="Return Icon" icon_class="icon brief-info__icon" role="presentation" focusable="false"}}
    </div>
    <div class="brief-info__content">
      <h3 class="brief-info__title">Return Policy</h3>
      <p class="brief-info__subtitle">Lorem Ipsum is simply</p>
    </div>

#### Popup product benefit 2 > popup-product-benefit-2

    <h2>Popup Product Benefit 2!</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel dui at dui rhoncus molestie. Praesent imperdiet semper gravida. Fusce ultricies dapibus magna, a fermentum purus viverra sed.</p>
    <p>Cras sed ultricies enim. Sed suscipit quis neque a porttitor. Phasellus aliquam ex ac mattis tincidunt. Lorem ipsum dolor sit amet, c</p>

#### Stock Status - More on the way > more_on_the_way

    More on the way content to be added via more_on_the_way cms block

#### Stock Status - Backordered > back_ordered

    Back ordered content to be added via back_ordered cms block

#### Stock Status - Custom Order > custom_order

    Custom order content to be added via custom_order cms block

#### Stock Status - Expanded Lead Time > expanded_lead_time

    Expanded Lead Time content to be added via expanded_lead_time cms block

#### Stock Status - Sold Out > sold_out

    Sold Out content to be added via sold_out cms block

#### In Stock popup content > one-day-shipping

    <h3 id="shipping-latency-title">The product is in stock</h3>
    <p>Usually shipps in less than 24 hours</p>

#### Menu - Category - Row with Images > menu-cat-images

    <ul class="list mega-menu__inner-list">
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper">
                    <img class="image lazyload" alt="Title 1" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 1
            </a>
        </li>
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper"><img class="image lazyload" alt="Title 2" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 2
            </a>
        </li>
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper"><img class="image lazyload" alt="Title 3" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 3
            </a>
        </li>
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper"><img class="image lazyload" alt="Title 4" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 4
            </a>
        </li>
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper"><img class="image lazyload" alt="Title 5" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 5
            </a>
        </li>
        <li class="list__item mega-menu__inner-item">
            <a class="link mega-menu__inner-link" tabindex="-1">
                <span class="lazyload-wrapper"><img class="image lazyload" alt="Title 6" data-src="{{config path="web/secure/base_url"}}media/wysiwyg/menu/160x160.jpg">
                </span>
                Title 6
            </a>
        </li>
    </ul>
