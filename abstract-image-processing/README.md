# [Abstract Image Processing](https://www.abstractapi.com/api/image-processing-optimization-api)

## __Description__
Manage your images programmatically with this powerful API: compress, convert, crop, resize, and more.

## __Example Request__
* Curl
```
curl https://images.abstractapi.com/v1/upload/ -X POST --form data='{api_key": "{{token}}", "lossy": true}' --form image=@path/to/image/file.jpg
```

* Raw
```
POST /v1/upload/ HTTP/1.1
Host: images.abstractapi.com
Content-Type: multipart/form-data; boundary=---abcd1234abcd1234abcd

---abcd1234abcd1234abcd
Content-Disposition: form-data; name="data"

{api_key": "{{token}}", "lossy": true}
---abcd1234abcd1234abcd
Content-Disposition: form-data; name="image"; filename="file.jpg"
Content-Type: image/jpeg

...................
...................
...................
...................
---abcd1234abcd1234abcd--
```

## __Response__
* Success
```
{
   "original_size": "the size of the original input image, in bytes",
   "original_height": "original height in pixels of the image",
   "original_width": "original width in pixels of the image",
   "final_size": "the size of the new image, in bytes",
   "bytes_saved": "the number of bytes saved by compressing and resizing the image",
   "final_height": "final height in pixels of the image",
   "final_width": "final width in pixels of the image",
   "url": "url of the image hosted by abstract for you to download. Images are available for 1 day.",
}
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fosc129sd241
```