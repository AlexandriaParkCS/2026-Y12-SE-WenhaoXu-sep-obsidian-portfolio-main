User

| Attribute    | Data Type | Bytes | Description                                                             | Example             |
| ------------ | --------- | ----- | ----------------------------------------------------------------------- | ------------------- |
| name         | String    | 256   | A free text name (actual name, initials, user selected username, etc.). | johnd, John Doe     |
| email        | String    | 64    | A valid email address.                                                  | john@abc.com        |
| pwd_hash     | String    | 128   | bycript hash of a password                                              | 5d41402abc4b2a76... |
| member since | Timestamp | 8     | The date and time when the user created their account.                  | 03/10/2025 16:38.42 |
