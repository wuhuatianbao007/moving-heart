
<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title></title>
    <style>
        body {
            /* background: greenyellow; */
            animation-name: pao;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }
        .box {
            margin: 100px auto;
            width: 300px;
            height: 300px;
            border: 20px solid #000;
            border-image: url("images/border_image_5.png") 19/19px 19px round;
            perspective: 300px;
        }
        .items {
            width: 300px;
            height: 300px;
            position: relative;
            perspective: 300px;
            animation-name: jump;
            animation-duration: 1s;
            animation-iteration-count: infinite;
        }
    .items div {
        width: 150px;
        height: 150px;
        background-color: red;
        position: absolute;
        left: 75px;
        top: 30px;
    }
        .item1,.item2 {
            border-radius: 75px 75px 0 0;
        }
        .item1 {
            transform: translate(-75px,0) rotate(-45deg);
        }
        .item2 {
            transform: translate(75px,0) rotate(45deg);
        }
        .item3 {
            transform: translate(0,75px) rotate(45deg);
        }
        @keyframes jump {
            from {
            }
            to{
                transform:  scale(1.5,1.5);
            }
        }
        @keyframes pao {
            from {
                background: url('images/paopao.png') no-repeat bottom right/cover, url('images/paopao.png') no-repeat top left/cover, hotpink;
            }
            to {
                background: url('images/paopao.png') no-repeat center left/cover, url('images/paopao.png') no-repeat bottom right/cover, skyblue;
            }
        }
    </style>
</head>
<!--<script>小宝是最棒的</script>-->
<body>
<div class="box">
    <div class="items">
        <div class="item1"></div>
        <div class="item2"></div>
        <div class="item3"></div>
    </div>
</div>
</body>
</html>
