## iauditor-exporter schema

Print iAuditor table schemas

### Synopsis

Print iAuditor table schemas

```
iauditor-exporter schema [flags]
```

### Examples

```
iauditor-exporter schema
```

### Options

```
  -h, --help   help for schema
```

### Options inherited from parent commands

```
  -t, --access-token string                 API Access Token
      --api-url string                      API URL (default "https://api.safetyculture.io")
      --config-path string                  config file (default "./.iauditor-exporter.yaml")
      --create-schema-only                  Create schema only (default false)
      --db-connection-string string         Database connection string
      --db-dialect string                   Database dialect. mysql, postgres and sqlserver are the only valid options. (default "mysql")
      --export-path string                  CSV Export Path (default "./export/")
      --inspection-archived string          Return archived inspections, false, true or both (default "false")
      --inspection-completed string         Return completed inspections, false, true or both (default "both")
      --inspection-include-inactive-items   Include inactive items in the inspection_items table (default false)
      --inspection-incremental-update       Update inspections, inspection_items and templates tables incrementally (default true)
      --inspection-skip-ids strings         Skip storing these inspection IDs
      --proxy-url string                    Proxy URL for making API requests through
      --tables strings                      Tables to export (default all)
      --template-ids strings                Template IDs to filter inspections and schedules by (default all)
      --tls-cert string                     Custom root CA certificate to use when making API requests
      --tls-skip-verify                     Skip verification of API TLS certificates
```

### SEE ALSO

* [iauditor-exporter](iauditor-exporter.md)	 - A CLI tool for extracting your iAuditor data

###### Auto generated by spf13/cobra on 24-Nov-2020