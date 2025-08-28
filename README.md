<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>موقعي لتعليم البرمجة</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background: black;
      color: #0f0;
      scroll-behavior: smooth;
    }

    /* بانر */
    .banner {
      position: relative;
      height: 100vh;
      width: 100%;
      background: url("mask.png") no-repeat center center/cover;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      overflow: hidden;
    }

    /* الأكواد الخضراء */
    .matrix {
      position: absolute;
      top: 0; left: 0;
      height: 100%; width: 100%;
      color: #0f0;
      font-size: 14px;
      white-space: pre;
      animation: move 10s linear infinite;
      opacity: 0.5;
    }
    @keyframes move {
      from { transform: translateY(-100%); }
      to { transform: translateY(100%); }
    }

    .content {
      position: relative;
      z-index: 2;
      color: #0f0;
    }

    .btn {
      margin-top: 20px;
      padding: 12px 24px;
      background: #0f0;
      color: black;
      font-weight: bold;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-decoration: none;
    }
    .btn:hover {
      background: red;
      color: #fff;
    }

    /* قسم الدروس */
    .lessons {
      padding: 50px 20px;
      background: #111;
    }
    .lesson {
      margin-bottom: 50px;
      padding: 20px;
      border: 1px solid #0f0;
      border-radius: 10px;
    }
    .lesson h2 {
      margin-top: 0;
    }
    pre {
      background: black;
      padding: 10px;
      overflow-x: auto;
      color: #0f0;
    }
  </style>
</head>
<body>

  <!-- بانر -->
  <div class="banner">
    <div class="matrix">
0100101101010010100101
1100101010110010010100
1010100101010101010101
0101100101001010101010
    </div>
    <div class="content">
      <h1>مرحباً بك في موقعي</h1>
      <p>تعلم البرمجة بأسلوب ممتع وسهل</p>
      <a href="#lessons" class="btn">ابدأ التعلم</a>
    </div>
  </div>

  <!-- قسم الدروس -->
  <div class="lessons" id="lessons">
    <div class="lesson" id="html">
      <h2>مقدمة في HTML</h2>
      <p>لغة HTML هي الهيكل الأساسي لأي صفحة ويب.</p>
      <pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
  &lt;head&gt;
    &lt;title&gt;مثال HTML&lt;/title&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;h1&gt;أهلاً بالعالم&lt;/h1&gt;
  &lt;/body&gt;
&lt;/html&gt;
      </pre>
    </div>

    <div class="lesson" id="css">
      <h2>أساسيات CSS</h2>
      <p>CSS بتتحكم في شكل الصفحة: الألوان، الأحجام، التنسيقات.</p>
      <pre>
body {
  background: black;
  color: white;
  font-family: Arial;
}
      </pre>
    </div>

    <div class="lesson" id="javascript">
      <h2>تعلم JavaScript</h2>
      <p>JavaScript بتدي تفاعلية للموقع زي الأزرار والحركات.</p>
      <pre>
&lt;script&gt;
  alert("مرحباً بك!");
&lt;/script&gt;
      </pre>
    </div>

    <div class="lesson" id="python">
      <h2>مقدمة في Python</h2>
      <p>Python من أسهل اللغات وأكثرها استخداماً في الذكاء الاصطناعي.</p>
      <pre>
print("Hello, World!")
      </pre>
    </div>

    <div class="lesson" id="java">
      <h2>مدخل إلى Java</h2>
      <p>Java قوية ومستخدمة في التطبيقات الكبيرة والهواتف.</p>
      <pre>
public class Main {
  public static void main(String[] args) {
    System.out.println("Hello, World!");
  }
}
      </pre>
    </div>
  </div>

</body>
</html>
