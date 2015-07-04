---
layout: post
title: New and Improved Website
categories: blog gamedev
---
I've finally got around to updating the design of my website!  

<div class="update">
<p><em>Update 07/04/2015:</em> This is a fake update.</p>
</div>

Here is a code block with the maximum code width (70 characters):

```c++

         1         2         3         4         5         6         7
1234567890123456789012345678901234567890123456789012345678901234567890
class Parser {
  public void register(TokenType token, PrefixParselet parselet) {
    mPrefixParselets.put(token, parselet);
  }

  public Expression parseExpression() {
    Token token = consume();
    PrefixParselet prefix = mPrefixParselets.get(token.getType());

    if (prefix == null) throw new ParseException(
        "Could not parse \"" + token.getText() + "\".");

    return prefix.parse(this, token);
  }

  // Other stuff...

  private final Map<TokenType, PrefixParselet> mPrefixParselets =
      new HashMap<TokenType, PrefixParselet>();
}
```

{% highlight c++ %}
void Movement::Movement
{
    m_position = 0.0f;
}

{% endhighlight %}


More text ...
