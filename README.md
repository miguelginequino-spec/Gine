<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Miguel — Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }

        body {
            background-color: #16213e;
            color: #ffffff;
            min-height: 100vh;
            padding: 2rem 4rem;
            line-height: 1.7;
            background-image: radial-gradient(circle at top left, #0f3460 0%, #16213e 70%);
        }

        /* Header & Profile Picture */
        .header-wrapper {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 1rem;
        }

        .profile-img {
            width: 120px;
            height: 10p0px;
            border-radius: 50%;
            object-fit: cover;
            border: 2px solid #98fb98;
            background-color: #98fb98;
        }

        .course-label {
            color: #98fb98;
            font-size: 1rem;
            font-weight: 400;
            margin-bottom: 0.3rem;
            letter-spacing: 0.5px;
        }

        h1 {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 0.2rem;
        }

        .tagline {
            font-size: 1.1rem;
            font-style: italic;
            color: #c9d1d9;
            margin-bottom: 1.5rem;
        }

        .btn-group {
            display: flex;
            gap: 1rem;
            margin-bottom: 2rem;
            flex-wrap: wrap;
        }

        .btn {
            padding: 0.6rem 1.4rem;
            border-radius: 6px;
            font-weight: 500;
            font-size: 0.95rem;
            border: none;
            cursor: pointer;
            transition: all 0.2s ease;
        }

        .btn-white {
            background: #ffffff;
            color: #16213e;
        }

        .btn-outline {
            background: transparent;
            color: #ffffff;
            border: 1px solid #ffffff;
        }

        .btn:hover {
            opacity: 0.9;
            transform: translateY(-1px);
        }

        .intro-text {
            background: rgba(255,255,255,0.05);
            padding: 1rem 1.2rem;
            border-radius: 6px;
            border-left: 2px solid #4cc9f0;
            margin-bottom: 2rem;
            font-size: 0.95rem;
            color: #e0e0e0;
        }

        .tags {
            display: flex;
            gap: 0.8rem;
            margin-bottom: 2rem;
            flex-wrap: wrap;
        }

        .tag {
            background: rgba(76, 201, 240, 0.15);
            color: #4cc9f0;
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* Grid Layout */
        .grid-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .card {
            background: rgba(255,255,255,0.05);
            border: 1px solid rgba(255,255,255,0.1);
            border-radius: 8px;
            padding: 1.3rem;
            backdrop-filter: blur(8px);
        }

        .card h3 {
            color: #98fb98;
            margin-bottom: 0.8rem;
            font-size: 1.1rem;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            padding-bottom: 0.3rem;
        }

        .card ul {
            list-style: none;
            padding-left: 0.5rem;
        }

        .card ul li::before {
            content: "•";
            color: #4cc9f0;
            font-weight: bold;
            display: inline-block;
            width: 1rem;
            margin-left: -1rem;
        }

        .card ul li {
            margin-bottom: 0.4rem;
            font-size: 0.9rem;
        }

        /* Education Section */
        .edu-item {
            margin-bottom: 1rem;
            padding-left: 0.8rem;
            border-left: 2px solid #4cc9f0;
        }

        .edu-year {
            font-size: 0.8rem;
            color: #a0a0a0;
        }

        .edu-course {
            font-weight: 600;
            font-size: 0.95rem;
        }

        .edu-school {
            font-size: 0.85rem;
            color: #d0d0d0;
        }

        /* Grade Checker */
        .grade-checker p {
            font-size: 0.85rem;
            color: #b0b0b0;
            margin-bottom: 0.7rem;
        }

        .input-group {
            display: flex;
            gap: 0.5rem;
            margin-bottom: 0.7rem;
        }

        #gradeInput {
            flex: 1;
            padding: 0.6rem 0.8rem;
            background: rgba(255,255,255,0.08);
            border: 1px solid rgba(255,255,255,0.2);
            border-radius: 4px;
            color: #fff;
        }

       
