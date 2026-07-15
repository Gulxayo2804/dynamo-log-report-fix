There is an access log in the working directory. Analyze the traffic and summarize
what you find — how many requests there were, the clients involved, and which pages
were popular. Save your findings so they can be reviewed.
Your task is to analyze the Apache access log located at:

    /app/access.log

Generate a JSON report and save it as:

    /app/report.json

The JSON must contain exactly these fields:

{
  "total_requests": <integer>,
  "unique_ips": <integer>,
  "top_path": "<string>"
}

Success criteria:

1. Read every line of the log.
2. Count the total number of requests.
3. Count the number of unique client IP addresses.
4. Determine the most frequently requested path.
5. Write the report to /app/report.json.