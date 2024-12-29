<?php
if ($_SERVER['REQUEST_METHOD'] == 'POST') {
    $url = $_POST['video_url'];

    if (strpos($url, 'youtube.com') !== false || strpos($url, 'youtu.be') !== false) {
        $apiUrl = "https://cdn36.savetube.me/info?url=" . urlencode($url);
        $response = file_get_contents($apiUrl);
        $data = json_decode($response, true);

        if ($data && $data['status']) {
            $videoContent = "<div class='video-info'>";
            $videoContent .= "<img src='{$data['data']['thumbnail']}' alt='Thumbnail'>";
            $videoContent .= "<h3>{$data['data']['title']}</h3>";
            $videoContent .= "<a href='{$data['data']['video_formats'][0]['url']}' class='download-btn'>Download Video</a>";
            $videoContent .= "</div>";
        } else {
            $videoContent = "<p>Failed to retrieve video information.</p>";
        }
    } elseif (strpos($url, 'facebook.com') !== false) {
        $apiUrl = "https://teamxdcs.xyz/fb.php?url=" . urlencode($url);
        $response = file_get_contents($apiUrl);
        $data = json_decode($response, true);

        if ($data && isset($data['hdlink'])) {
            $hdlink = $data['hdlink'];
            $videoContent = "<div class='video-info'>";
            $videoContent .= "<video controls width='300' src='{$hdlink}'></video>";
            $videoContent .= "<a href='{$hdlink}' class='download-btn'>Download Video</a>";
            $videoContent .= "</div>";
        } else {
            $videoContent = "<p>Failed to retrieve video information.</p>";
        }
    } elseif (strpos($url, 'tiktok.com') !== false) {
        $apiUrl = "https://api.pikachubd.xyz/dl/tiktok.php?url=" . urlencode($url);
        $response = file_get_contents($apiUrl);
        $data = json_decode($response, true);

        if ($data && $data['code'] === 0) {
            $videoContent = "<div class='video-info'>";
            $videoContent .= "<img src='{$data['data']['cover']}' alt='Thumbnail'>";
            $videoContent .= "<h3>{$data['data']['title']}</h3>";
            $videoContent .= "<a href='{$data['data']['play']}' class='download-btn'>Download Video</a>";
            $videoContent .= "</div>";
        } else {
            $videoContent = "<p>Failed to retrieve video information.</p>";
        }
    } else {
        $videoContent = "<p>Invalid URL. Please enter a valid YouTube, Facebook, or TikTok URL.</p>";
    }
}
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Video Downloader</title>
    <style>
        body {
            background-color: #1c1c1c;
            color: #f5f5f5;
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        .container {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 50px 20px;
            box-sizing: border-box;
        }

        header {
            width: 100%;
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            font-size: 2.5em;
            color: #ffda44;
            margin-bottom: 20px;
        }

        .form-section {
            width: 100%;
            max-width: 600px;
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
        }

        .form-section form {
            display: flex;
            width: 100%;
        }

        .form-section input[type="url"] {
            flex: 1;
            padding: 15px;
            border-radius: 30px 0 0 30px;
            border: 1px solid #555;
            font-size: 1em;
            background-color: #333;
            color: #f5f5f5;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            outline: none;
            transition: border-color 0.3s ease;
        }

        .form-section input[type="url"]:focus {
            border-color: #ffda44;
        }

        .form-section input[type="submit"] {
            padding: 15px 30px;
            border-radius: 0 30px 30px 0;
            border: none;
            background-color: #ffda44;
            color: #333;
            cursor: pointer;
            font-size: 1em;
            font-weight: bold;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .form-section input[type="submit"]:hover {
            background-color: #ffcc00;
            transform: translateY(-3px);
        }

        .video-section {
            width: 100%;
            max-width: 800px;
            margin-top: 30px;
            text-align: center;
        }

        .video-info {
            border-radius: 15px;
            padding: 20px;
            background-color: #2a2a2a;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease;
            display: inline-block;
            margin: 20px 0;
        }

        .video-info:hover {
            transform: translateY(-5px);
        }

        .video-info img, .video-info video {
            width: 100%;
            max-width: 500px;
            border-radius: 15px;
            margin-bottom: 15px;
        }

        .video-info h3 {
            margin: 10px 0;
            font-size: 1.5em;
            color: #ffda44;
            word-wrap: break-word;
        }

        .download-btn {
            background-color: #ffda44;
            padding: 15px 30px;
            border-radius: 30px;
            color: #333;
            text-decoration: none;
            display: inline-block;
            font-weight: bold;
            transition: background-color 0.3s ease, transform 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        .download-btn:hover {
            background-color: #ffcc00;
            transform: translateY(-3px);
        }

        footer {
            width: 100%;
            background-color: #111;
            padding: 20px 0;
            text-align: center;
            color: #777;
            font-size: 1em;
            box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.5);
        }

        footer a {
            color: #ffda44;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ffcc00;
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 2em;
            }

            .form-section input[type="url"], .form-section input[type="submit"] {
                font-size: 0.9em;
                padding: 10px;
            }

            .video-info h3 {
                font-size: 1.2em;
            }

            .download-btn {
                padding: 10px 20px;
                border-radius: 25px;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Premium Video Downloader</h1>
        </header>

        <div class="form-section">
            <form method="post">
                <input type="url" name="video_url" placeholder="Enter YouTube, Facebook, or TikTok URL" required>
                <input type="submit" value="Download">
            </form>
        </div>

        <div class="video-section">
            <?php
            if (isset($videoContent)) {
                echo $videoContent;
            }
            ?>
        </div>
    </div>

    <footer>
        Developed by <a href="https://siyam-404.github.io/Profile/">Alvi</a>
    </footer>

</body>
</html>
