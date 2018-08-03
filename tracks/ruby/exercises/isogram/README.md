### Possible model solution

```ruby
def isogram?(string)
  letters = string.downcase.scan(/[a-z]/)
  letters.uniq.length == letters.length
end
```

### Common suggestions
- Suggest using `scan` rather than `gsub` as it removes the need to break the string into chars. Links to https://ruby-doc.org/core-2.2.0/String.html#method-i-scan

### Talking points
- Comparing lengths is **marginally** quicker than comparing but its more code. Which is better?