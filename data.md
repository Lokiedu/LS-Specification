# Data types

  
Some objects which contain a vast set of fields are used for whole groups of methods at a time. Below are the links to pages with detailed description of such objects

### [ ](https://github.com/Lokiedu/libertysoil-site/wiki/Attachment-object)[Attachment](https://github.com/Lokiedu/libertysoil-site/wiki/Attachment-object)

```
Attachment = {
  attachment_id: String (required),
  url: String (url; required)
}
```

### [Hashtag](https://github.com/Lokiedu/libertysoil-site/wiki/Hashtag-object)

```
Hashtag = {
  created_at: String (date representation; required),
  id: String (uuid4; required),
  name: String (url; required),
  more: TagMore,
  post_count: Number (required),
  updated_at: String (date representation; required)
}
```

### [Geotag](https://github.com/Lokiedu/libertysoil-site/wiki/Geotag-object)

```
Geotag = {
  admin: Geotag,
  admin1_code: String,
  admin1_id: String (uuid4),
  continent: Geotag,
  continent_code: String (one of continents codes: "EU", "AS", "NA", "SA", "OC", "AF", "AN"),
  continent_id: String (uuid4),
  country: Geotag,
  country_code: String,
  country_id: String (uuid4),
  created_at: String (date representation; required),
  geonames_admin1_id: Number,
  geonames_city_id: Number,
  geonames_country_id: Number,
  geonames_id: String,
  id: String (uuid4; required),
  land_mass: Number,
  lat: Number,
  lon: Number,
  more: TagMore,
  name: String (required),
  post_count: Number (required),
  type: String (potentially one of "Country", "Continent", "AdminDivision1", or similar; needs improvement),
  updated_at: String (date representation; required),
  url_name: String (url; required)
}
```

### [School](https://github.com/Lokiedu/libertysoil-site/wiki/School-object)

```
School = {
  address1: String,
  address2: String,
  city: String,
  country_id: String (uuid4),
  created_at: String (date representation; required),
  description: String,
  facebook: String,
  foundation_day: Number,
  foundation_month: Number,
  foundation_year: Number,
  house: String,
  id: String (uuid4; required),
  images: Array[Attachment],
  is_open: Boolean,
  lat: Number,
  lon: Number,
  more: TagMore,
  name: String (required),
  number_of_students: Number,
  org_membership: {},
  phone: String,
  post_count: Number (required),
  postal_code: String,
  principal_name: String,
  principal_surname: String,
  required_languages: Array[String],
  teaching_languages: Array[String],
  twitter: String,
  updated_at: String (date representation; required),
  url_name: String (url; required),
  website: String,
  wikipedia: String
}
```

`LightSchool`comes with each post as related tag instead of full version of School

```
LightSchool = {
  id: String (uuid4; required),
  url_name: String (url; required),
  name: String (required)
});
```

### [TagMore](https://github.com/Lokiedu/libertysoil-site/wiki/TagMore-object)

```
TagMore = {
  description: String,
  head_pic: Attachment,
  last_editor: String (uuid4)
}
```



