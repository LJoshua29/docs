
{% endraw %

For more information, see "[Configuration options for the dependabot.yml file](/github/administering-a-repository/configuration-options-for-dependency-updates#configuration-options-for-private-registries)."

### Naming your secrets

* Can only contain alphanumeric characters (`[A-Z]`, `[0-9]`) or underscores (`_`). Spaces are not allowed. If you 

{% data reusables.actions.sidebar-p
{% data reusables.dependabot.dependabot-secrets-button %}
1. Click **New organization secret**.
1. Type a name for your secret in the **:

   * Click {% octicon "gear" aria-label="The Gear icon" %}.
   * Choose the repositories that can access this secret. 
     ![Select repositories for this secret](/assets/images/help/dependabot/secret-repository-access.png)
   * Click **Update selection**.

1. Click **Add secret**.

   The name of the secret is listed on the Dependabot secrets page. You can click **Update** to change the secret value or its access policy. You can click **Remove** to delete the secret.

   ![Update or remove an organization secret](/assets/images/help/dependabot/update-remove-org-secret.png)
   
## Adding {% data variables.product.prodname_dependabot %} to your registries IP allow list

If your private registry is configured with an IP allow list, you can find the IP addresses {% data variables.product.prodname_dependabot %} uses to access the registry in the meta API endpoint, under the `dependabot` key. For more information, see "[Meta](/rest/reference/meta)."
