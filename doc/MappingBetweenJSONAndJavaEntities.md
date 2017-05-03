| JSON       | Java              |
| :--------- | :---------------- |
| string     | java.lang.String  |
| number     | java.lang.Number  |
| true|false | java.lang.Boolean |
| null       | null              |
| array      | java.util.List    |
| object     | java.util.Map     |

JSON.simple maps entities from the left side to the right side while decoding or parsing, and maps entities from the right to the left while encoding. While decoding, default concrete class of java.util.List is org.json.simple.JSONArray and default concrete class of java.util.Map is org.json.simple.JSONObject. While encoding, other classes that are not listed on the right side of the table need to implement JSONAware or JSONStreamAware (streaming only) to [customize](EncodingExamples.md) JSON outputs. In such cases, JSON.simple calls JSONAware.toJSONString() or JSONStreamAware.writeJSONString() to determine the resulting JSON text.
