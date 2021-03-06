# resume_exporter

``` sh
resumeExporter --target TARGET [-h] [--source_ids [SOURCE_IDS [SOURCE_IDS ...]]]
                          [--api_key API_KEY] [--verbose]
                          [--silent] [--n-worker N_WORKER] [--logfile LOGFILE]
```

## Description
  resume_exporter get profile's documents of candidates and profile parsing from the sources that you selected.
  These documents are dump in the target directory you selected under the following path: `$taget_path/$source_name_$source_id/$profile_id/*`

## Options
* --target path/to/target/directory
  * Directory where profile's files will be dump
  * **Required**
* -h
  * print help message and exit
* --source_ids source_id1 source_id2 ... source_idn
  * Source ids from where profile will be exported.
  * **Default**: All sources available with your secret key are selected by default.
* --api_key api_secret_key
  * Your api secret, available on your riminder platform.
  * Will be asked if absent.
* --api_url api_url
  * The url to the riminder api
  * **Default** "https://www.riminder.net/sf/public/api/v1.0/"
* --verbose
  * Enable verbose mode
* --silent
  * Enable silent mode
* --n-worker n
  * Select the number of worker (thread) you want to use.
  * **Default**: 3
* --logfile path/to/file
  * Select a file where export logs will be logged

