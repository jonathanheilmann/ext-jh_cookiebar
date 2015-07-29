.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. include:: ../Includes.txt


.. _configuration:

Configuration
=============

.. _configuration-typoscript:

TypoScript Reference
--------------------

All importend configuration may be done in Constants Editor. For advanced configuration please see advanced configuration


Properties
^^^^^^^^^^

.. container:: ts-properties

   =========================== ===================================== ======================= ================================================================================= 
   Property                    Data type                             :ref:`t3tsref:stdwrap`  Default
   =========================== ===================================== ======================= ================================================================================= 
	css_                        :ref:`t3tsref:data-type-string`       no                      EXT:jh\_cookiebar\/Resources\/Public\/Styles\/jquery.cookiebar.css
   js_                         :ref:`t3tsref:data-type-string`       no                      EXT:jh\_cookiebar\/Resources\/Public\/Contrib\/CookieBar\/jquery.cookiebar.min.js
	template_                   :ref:`t3tsref:data-type-string`       no                      EXT:jh\_cookiebar\/Resources\/Private\/Templates\/TypoScript\/Default.html
   policyUrl_                  :ref:`t3tsref:data-type-int`          no
   acceptButton_               :ref:`t3tsref:data-type-boolean`      no                      0
   policyButton_               :ref:`t3tsref:data-type-boolean`      no                      0
   autoEnable_                 :ref:`t3tsref:data-type-boolean`      no                      1
   acceptOnContinue_           :ref:`t3tsref:data-type-boolean`      no                      0
   acceptOnScroll_             :ref:`t3tsref:data-type-boolean`      no                      0
   acceptAnyClick_             :ref:`t3tsref:data-type-boolean`      no                      0
   expireDays_                 :ref:`t3tsref:data-type-int`          no                      365
   renewOnVisit_               :ref:`t3tsref:data-type-boolean`      no                      0
   forceShow_                  :ref:`t3tsref:data-type-boolean`      no                      0
   effect_                     :ref:`t3tsref:data-type-string`       no                      slide
   fixed_                      :ref:`t3tsref:data-type-boolean`      no                      0
   bottom_                     :ref:`t3tsref:data-type-boolean`      no                      0
   zindex_                     :ref:`t3tsref:data-type-int`          no
   =========================== ===================================== ======================= =================================================================================


Property details
^^^^^^^^^^^^^^^^

.. only:: html

	.. contents::
		:local:
		:depth: 1


.. _ts-plugin-tx-jhcookiebar-settings-css:

css
"""

:typoscript:`plugin.tx_jhcookiebar.settings.css =` :ref:`t3tsref:data-type-string`

CSS file to style the CookieBar


.. _ts-plugin-tx-jhcookiebar-settings-js:

js
""

:typoscript:`plugin.tx_jhcookiebar.settings.js =` :ref:`t3tsref:data-type-string`

JS file of the CookieBar


.. _ts-plugin-tx-jhcookiebar-settings-template:

template
""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.template =` :ref:`t3tsref:data-type-string`

JavaScript template to initialise CookieBar


.. _ts-plugin-tx-jhcookiebar-settings-policyUrl:

policyUrl
"""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.policyUrl =` :ref:`t3tsref:data-type-int`

Id of Privacy Policy page (**Required when policyButton is enabled**)


.. _ts-plugin-tx-jhcookiebar-settings-acceptButton:

acceptButton
""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.acceptButton =` :ref:`t3tsref:data-type-boolean`

Set to true to show accept/enable button


.. _ts-plugin-tx-jhcookiebar-settings-policyButton:

policyButton
""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.policyButton =` :ref:`t3tsref:data-type-boolean`

Set to true to show Privacy Policy button


.. _ts-plugin-tx-jhcookiebar-settings-autoEnable:

autoEnable
""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.autoEnable =` :ref:`t3tsref:data-type-boolean`

Set to true for cookies to be accepted automatically. Banner still shows


.. _ts-plugin-tx-extensionkey-acceptOnContinue:

acceptOnContinue
""""""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.acceptOnContinue =` :ref:`t3tsref:data-type-boolean`

Set to true to accept cookies when visitor moves to another page


.. _ts-plugin-tx-jhcookiebar-settings-acceptOnScroll:

acceptOnScroll
""""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.acceptOnScroll =` :ref:`t3tsref:data-type-boolean`

Set to true to accept cookies when visitor scrolls X pixels up or down


.. _ts-plugin-tx-jhcookiebar-settings-acceptAnyClick:

acceptAnyClick
""""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.acceptAnyClick =` :ref:`t3tsref:data-type-boolean`

Set to true to accept cookies when visitor clicks anywhere on the page


.. _ts-plugin-tx-jhcookiebar-settings-expireDays:

expireDays
""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.expireDays =` :ref:`t3tsref:data-type-int`

Number of days for cookieBar cookie to be stored for


.. _ts-plugin-tx-jhcookiebar-settings-renewOnVisit:

renewOnVisit
""""""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.renewOnVisit =` :ref:`t3tsref:data-type-boolean`

Renew the cookie upon revisit to website


.. _ts-plugin-tx-jhcookiebar-settings-forceShow:

forceShow
"""""""""

:typoscript:`plugin.tx_jhcookiebar.settings.forceShow =` :ref:`t3tsref:data-type-boolean`

Force cookieBar to show regardless of user cookie preference 


.. _ts-plugin-tx-jhcookiebar-settings-effect:

effect
""""""

:typoscript:`plugin.tx_jhcookiebar.settings.effect =` :ref:`t3tsref:data-type-string`

Options: slide, fade, hide


.. _ts-plugin-tx-jhcookiebar-settings-fixed:

fixed
"""""

:typoscript:`plugin.tx_jhcookiebar.settings.fixed =` :ref:`t3tsref:data-type-boolean`

Set to true to add the class "fixed" to the cookie bar. Default CSS should fix the position


.. _ts-plugin-tx-jhcookiebar-settings-bottom:

bottom
""""""

:typoscript:`plugin.tx_jhcookiebar.settings.bottom =` :ref:`t3tsref:data-type-boolean`

Force CSS when fixed, so bar appears at bottom of website


.. _ts-plugin-tx-jhcookiebar-settings-zindex:

zindex
""""""

:typoscript:`plugin.tx_jhcookiebar.settings.zindex =` :ref:`t3tsref:data-type-int`

Can be set in CSS, although some may prefer to set here


.. _configuration_advanced-configuration

Advanced Configuration
----------------------

The JavaScript to initialise CookieBar is created in a tempalte located at: EXT:jh_cookiebar/Resources/Private/Templates/TypoScript/Default.html

To use your own modified template change the value of template_.

.. code-block:: html
   
   ;(function($){
      $(document).ready(function(){
         $.cookieBar({
            message: '<f:translate key="jquery.cookiebar.message" extensionName="JhCookiebar" />',
            acceptButton: {settings.acceptButton},
            acceptText: '<f:translate key="jquery.cookiebar.acceptText" extensionName="JhCookiebar" />',
            declineButton: 0,
            policyButton: {settings.policyButton},
            policyText: '<f:translate key="jquery.cookiebar.policyText" extensionName="JhCookiebar"/>',
            policyURL: '{policyUrl}',
            autoEnable: {settings.autoEnable},
            acceptOnContinue: {settings.acceptOnContinue},
            acceptOnScroll: {settings.acceptOnScroll},
            acceptAnyClick: {settings.acceptAnyClick},
            expireDays: {settings.expireDays},
            renewOnVisit: {settings.renewOnVisit},
            forceShow: {settings.forceShow},
            effect: '{settings.effect}',
            fixed: {settings.fixed},
            bottom: {settings.bottom},
            zindex: {settings.zindex},
            domain: '{domain}',
            referrer: '{referrer}'
         });
      });
   })(jQuery);
   
   
.. _configuration_translation

Translation
-----------

To translate the labels/texts of the extension use TypoScript setup, too.

Default labels:

.. code-block:: typoscript
   
   plugin.tx_jhcookiebar._LOCAL_LANG {
      default {
         jquery.cookiebar.message = We use cookies to personalise content and ads, to provide social media features and to analyse our traffic. We also share information about your use of our site with our social media, advertising and analytics partners.
         jquery.cookiebar.acceptText = Got it
         jquery.cookiebar.policyText = See details
      }
      de {
         jquery.cookiebar.message = Wir verwenden Cookies, um Inhalte und Anzeigen zu personalisieren, Funktionen für soziale Medien anbieten zu können und die Zugriffe auf unsere Website zu analysieren. Außerdem geben wir Informationen zu Ihrer Nutzung unserer Website an unsere Partner für soziale Medien, Werbung und Analysen weiter.
         jquery.cookiebar.acceptText = OK
         jquery.cookiebar.policyText = Details ansehen
      }
   }