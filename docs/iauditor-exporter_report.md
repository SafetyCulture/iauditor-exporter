## iauditor-exporter report

Export inspection report

### Synopsis

Export inspection report

```
iauditor-exporter report [flags]
```

### Examples

```
// Export PDF and Word inspection reports
		iauditor-exporter report --export-path /path/to/export/to --format PDF,WORD
		// Export PDF inspection reports with a custom report preference
		iauditor-exporter report --export-path /path/to/export/to --format PDF --preference-id abc
```

### Options

```
  -t, --access-token string                 API Access Token
      --api-url string                      API URL (default "https://api.safetyculture.io")
      --export-path string                  CSV Export Path (default "./export/")
      --format strings                      Export format (PDF,WORD)
  -h, --help                                help for report
      --inspection-archived string          Return archived inspections, false, true or both (default "false")
      --inspection-completed string         Return completed inspections, false, true or both (default "both")
      --inspection-include-inactive-items   Include inactive items in the inspection_items table (default false)
      --inspection-incremental-update       Update inspections, inspection_items and templates tables incrementally (default true)
      --inspection-modified-after string    Return inspections modified after this date
      --inspection-skip-ids strings         Skip storing these inspection IDs
      --preference-id string                The report preference to apply to the document
      --proxy-url string                    Proxy URL for making API requests through
      --template-ids strings                Template IDs to filter inspections and schedules by (default all)
      --tls-cert string                     Custom root CA certificate to use when making API requests
      --tls-skip-verify                     Skip verification of API TLS certificates
```

### Options inherited from parent commands

```
      --config-path string   config file (default "./iauditor-exporter.yaml")
```

### SEE ALSO

* [iauditor-exporter](iauditor-exporter.md)	 - A CLI tool for extracting your iAuditor data

###### Auto generated by spf13/cobra on 29-Jan-2021
