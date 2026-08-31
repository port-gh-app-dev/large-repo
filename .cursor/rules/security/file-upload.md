# File Upload Security Rules

- Deny uploads by default and allow only required MIME types/extensions.
- Validate file type using both MIME sniffing and content signatures (magic bytes).
- Enforce strict file size limits and request body limits.
- Rename uploaded files to generated IDs; never trust client-provided filenames.
- Store uploads outside executable/static web roots when possible.
- Scan uploads with malware detection before downstream processing.
- Strip metadata from media files when privacy/security requires it.
- Prevent path traversal by normalizing and validating storage paths.
- Use isolated storage buckets/containers with least-privilege access.
- For public downloads, serve files through controlled handlers with authorization checks.
