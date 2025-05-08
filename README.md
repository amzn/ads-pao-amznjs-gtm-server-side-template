# Amazon Ad Tag Server-Side Template for Google Tag Manager

This Google Tag Manager server-side template allows you to implement Amazon Advertising tags on your website using Google Tag Manager's server-side capabilities.

## Key Features

- Operates on GA4 events
- Supports Measurement Token, an ID-less way of attributing ad clicks to a user
- Supports Match ID, enabling mapping of ID-less events to ID-have events via a user-unique value
  - This feature is especially helpful when an advertiser only obtains user information part of the way through their flow

## Installation

1. In your Google Tag Manager server container, go to Templates
2. Click "New" to create a new template
3. Click "Import" and select the template.tpl file from this repository
4. Save the template

## Configuration

After importing the template, you can create a new tag using this template. The tag configuration includes:

1. Amazon Ad Tag IDs
2. Event Name (standard or custom)
3. Region selection
4. Advanced Matching for User Data (optional)
5. Off-Amazon Purchase Attributes (for Off-Amazon Purchase events)
6. Default and Custom Attributes
7. TCFv2 settings (optional)
8. Amazon Consent settings

## Usage

The tag will fire based on your configured triggers, typically on GA4 events. It handles:

- Token generation and management
- Sending event data to Amazon's advertising platform
- Applying consent settings as configured

## Advanced Features

- Measurement Token handling for cookieless attribution
- Match ID support for connecting anonymous and identified user events
- TCFv2 and Amazon Consent integrations for privacy compliance

## Support

For issues, questions, or contributions, please open an issue or pull request in this repository.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This project is licensed under the Apache-2.0 License.