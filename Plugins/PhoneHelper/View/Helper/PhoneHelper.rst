--------------------------------------
PhoneHelper\\View\\Helper\\PhoneHelper
--------------------------------------

.. php:namespace: PhoneHelper\\View\\Helper

.. php:class:: PhoneHelper

    PhoneHelper Main Class

    This class extends the NumberHelper built into CakePHP 3.x and adds the ability to parse and prettify a US telephone number.

    .. php:attr:: _defaultConfig

        protected array

        Default config for this class

    .. php:method:: format($number)

        Prettify a phone number.

        This function can take either a 10 digit or 7 digit phone number and
        returns a more human readable version.

        :type $number: int
        :param $number: The phone number to be prettified
        :returns: string The prettified phone number

    .. php:method:: link($title, $url = null, $options = [])

        Creates an HTML telephone link.

        If the $url is empty, $title is used instead.

        ### Options

        - `escape` Set to false to disable escaping of title and attributes.
        - `escapeTitle` Set to false to disable escaping of title. Takes
        precedence over value of `escape`)

        :type $title: string
        :param $title: The content to be wrapped by `<a>` tags.
        :type $url: string|null
        :param $url: string The phone number to link to.
        :type $options: array
        :param $options: Array of options and HTML attributes.
        :returns: string An `<a />` element.

    .. php:method:: buildUrl($url)

        Builds a telephone link from a passed in string

        The string passed in can be a number, formatted number, or tel url

        :type $url: string
        :param $url: The number or tel url to use in the link
        :returns: string rfc3966 formatted tel URL
