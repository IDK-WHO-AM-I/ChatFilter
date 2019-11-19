# ChatFilter

---

This is a public list for badwords used by my ChatFilter Plugin!
You wanna try my plugin? Contact me via mail

---

You wanna use this list yourself?

Here a method how you can get get a List of these bad words:


```java

    private Gson gson = new GsonBuilder().serializeNulls().setPrettyPrinting().create();

    public List<String> getBadWords() throws IOException {
        URL url = new URL("https://raw.githubusercontent.com/IDK-WHO-AM-I/ChatFilter/master/words.json");
        try (BufferedReader reader = new BufferedReader(new InputStreamReader(url.openStream()))) {
            return gson.fromJson(reader, new TypeToken<List<String>>() {
            }.getType());
        }
    }
  ```
  ---
