---
title: Enabling automatic access to GitHub.com actions using GitHub Connect
intro: 'To allow {{ site.data.variables.product.prodname_actions }} on your enterprise instance to use actions from {{ site.data.variables.product.prodname_dotcom_the_website }}, you can connect {{ site.data.variables.product.product_location_enterprise }} to {{ site.data.variables.product.prodname_ghe_cloud }}.'
permissions: 'Site administrators for {{ site.data.variables.product.prodname_ghe_server }} who are also owners of the connected {{ site.data.variables.product.prodname_ghe_cloud }} organization or enterprise account can enable access to all {{ site.data.variables.product.prodname_dotcom_the_website }} actions.'
redirect_from:
  - /enterprise/admin/github-actions/enabling-automatic-access-to-githubcom-actions-using-github-connect
versions:
  enterprise-server: '>=2.22'
---

{{ site.data.reusables.actions.enterprise-beta }}
{{ site.data.reusables.actions.enterprise-github-hosted-runners }}

By default, {{ site.data.variables.product.prodname_actions }} workflows on {{ site.data.variables.product.prodname_ghe_server }} cannot use actions directly from {{ site.data.variables.product.prodname_dotcom_the_website }} or [{{ site.data.variables.product.prodname_marketplace }}](https://github.com/marketplace?type=actions).

To make all actions from {{ site.data.variables.product.prodname_dotcom_the_website }} available on your enterprise instance, you can connect {{ site.data.variables.product.prodname_ghe_server }} to {{ site.data.variables.product.prodname_ghe_cloud }} using {{ site.data.variables.product.prodname_github_connect }}. For other ways of accessing actions from {{ site.data.variables.product.prodname_dotcom_the_website }}, see "[About using {{ site.data.variables.product.prodname_dotcom_the_website }} actions on {{ site.data.variables.product.prodname_ghe_server }}](/enterprise/admin/github-actions/about-using-githubcom-actions-on-github-enterprise-server)."

### Enabling automatic access to all {{ site.data.variables.product.prodname_dotcom_the_website }} actions

Before enabling access to all actions from {{ site.data.variables.product.prodname_dotcom_the_website }} on {{ site.data.variables.product.product_location_enterprise }}, you must connect {{ site.data.variables.product.product_location_enterprise }} to {{ site.data.variables.product.prodname_dotcom_the_website }}. Weitere Informationen finden Sie unter „[{{ site.data.variables.product.prodname_ghe_server }} mit {{ site.data.variables.product.prodname_ghe_cloud }} verbinden](/enterprise/{{ currentVersion }}/admin/guides/installation/connecting-github-enterprise-server-to-github-enterprise-cloud)“.

{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.business }}
{{ site.data.reusables.enterprise-accounts.settings-tab }}
{{ site.data.reusables.enterprise-accounts.github-connect-tab }}
1. Under "Server can use actions from GitHub.com in workflows runs", use the drop-down menu and select **Enabled**. ![Drop-down menu to actions from GitHub.com in workflows runs](/assets/images/enterprise/site-admin-settings/enable-marketplace-actions-drop-down.png)