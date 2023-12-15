<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="SalesReport.aspx.cs" Inherits="Final_Project_Bell.Design.SalesReport" %>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
    <title></title>
    <style type="text/css">
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(45deg, black, gold);
        }

        .auto-style1 {
            height: 600px;
            width: 1250px;
            /* Additional styles for the form container if needed */
            background-color: rgba(255, 255, 255, 0.8); /* Example: Semi-transparent white background for the form */
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            text-align: center;
        }

        #sidebar {
      width: 250px;
      height: 100%;
      background-color: #333;
      position: fixed;
      left: 0;
      top: 0;
      padding-top: 20px;
    }

    #sidebar a {
      text-decoration: none;
      font-size: 18px;
      color: #fff;
      display: block;
      padding: 10px;
      transition: 0.3s;
    }

    #sidebar a:hover {
      background-color: #555;
    }



    #menu-btn {
      font-size: 24px;
      cursor: pointer;
      position: fixed;
      left: 20px;
      top: 20px;
      color: #fff;
      z-index: 1;
    }
        .auto-style2 {
            left: 0;
            top: -138px;
            height: 63%;
            text-align: center;
        }
        .auto-style3 {
            text-align: justify;
        }
    </style>
</head>
<body>
    <form id="form1" runat="server" class="auto-style1">
        <div class="auto-style3">
        <div id="sidebar" class="auto-style2" style="font-family: 'Arial Black'">
  <a href="#">Home</a>
  <a href="#">Dashboard</a>
  <a href="#">Inventory</a>
  <a href="#">Sales</a>
  <a href="#">Purchases</a>
  <a href="#">Transactions</a>
&nbsp;</div>



<script>
    document.getElementById("menu-btn").addEventListener("click", function () {
        document.getElementById("sidebar").style.width = "250px";
        document.getElementById("content").style.marginLeft = "250px";
    });

        document.getElementById("sidebar").style.width = "0";
        document.getElementById("content").style.marginLeft = "0";
    });
</script>
        </div>
        </form>
</body>
</html>
