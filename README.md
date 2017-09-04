# sweeping-effect
css to make sweeping effect
```
<!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title> css to make sweeping effect</title>
      <style>
        p {
          position: relative;
          width: 200px;
          height: 40px;
          line-height: 40px;
          text-align:center;
          background: blue;
          font-size: 28px;
          color: #fff;
          animation: sweepingEffect 2s ease infinite;
        }
        p:before {
          content: '';
          position:absolute;
          top: -300px;
          left: -300px;
          width: 200px;
          height: 20px;
          background: #fff;
          box-shadow: 10px 10px 10px #fff;
          transfrom: rotateZ(45deg);
        }
        @keyframes sweepingEffect {
          0%,75% {top: 0; left: -100%}
          100% {top: 100px; left: 100%}
        }
      </style>
    </head>
    <body>
      <p> css to make sweeping effect></p>
    </body>
 </html>
```
