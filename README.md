# Rich-Interview

You have been assigned a bug in a legacy system that uses an archived gem called `global_phone`.

https://github.com/sstephenson/global_phone

The bug ticket you're working on says that the form accepts numbers with too many digits. The example given:

```
Guatemala has eight-digit phone numbers, but the number "5555 1234 123" still gets through the matcher.
```

The app you're working on allows users to register with a phone number. The user's country is inferred from the country code in the phone number.

- GlobalPhone.parse('5555 1234 123') # => an object that specifies the country, and the way the phone number would be formatted in that country.
- GlobalPhone.validate('5555 1234 123') # => a boolean that says whether this looks like a correct phone number
- GlobalPhone.normalize('5555 1234 123') # => normalizes to E.164 format to store to the database

