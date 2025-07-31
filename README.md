# online-course-tech
Advance your career with expert-led aviation courses—pilot training, safety, and management. Explore digital marketing and AI, all on one easy-to-use platform. Build your personal brand as you learn. Transform your future, one course at a time.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Online Course Platform</title>
  <link rel="stylesheet" href="styles.css" />
  <style>
  body {
  font-family: Arial, sans-serif;
  padding: 20px;
  background: #87CEFA;
  color: #333;
}

.container {
  max-width: 800px;
  margin: 0 auto;
  background: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgb(0 0 0 / 0.1);
  background-color: white;
}

.category-list {
  list-style: none;
  padding: 0;
  display: flex;
  gap: 15px;
  margin-bottom: 30px;
}

.category-list li {
  cursor: pointer;
  padding: 10px 15px;
  background: #e1e4ea;
  border-radius: 20px;
  transition: background 0.3s;
}

.category-list li.active,
.category-list li:hover {
  background: #007bff;
  color: white;
}

.course-list {
  list-style: none;
  padding: 0;
}

.course-list li {
  margin-bottom: 25px;
  padding-bottom: 15px;
  border-bottom: 1px solid #ddd;
}

.course-title {
  margin: 0 0 8px 0;
  font-size: 1.2em;
}

.course-description {
  margin: 0 0 8px 0;
}

.video {
  width: 250px;
  height: 400px;
}

.instructor {
  font-style: italic;
  font-size: 0.9em;
  color: #555;
}

/*h1*/

.gradient-text {
      color: black;
      display: flex;
      align-items: center;
      font-size: 50px;
 }

.name {
  display: flex;
        align-items: center;
        justify-content: space-between;
}

.name img {
  height: 100px;
  width: 100px;
  border-radius: 50px;  
}

/*about boss*/

    .about-boss {
      margin-top: 48px;
      background: linear-gradient(#F0FFFF, #87CEFA);
      -webkit-background-clip: background;
      padding: 24px 28px;
      border-radius: 15px;
      box-shadow: inset 0 0 10px rgba(64, 132, 255, 0.12);
      display: flex;
      gap: 20px;
      align-items: center;
      max-width: 900px;
      margin-left: auto;
      margin-right: auto;
    }
    .boss-photo {
      width: 110px;
      height: 110px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #2575fc;
    }
    .boss-info {
      flex: 1;
    }
    .boss-info h3 {
      margin-bottom: 4px;
      color: #1e2e54;
    }
    .boss-info p {
      margin-bottom: 4px;
      font-size: 1rem;
      color: #3f4a72;
    }
    .boss-info a {
      color: #2575fc;
      text-decoration: none;
      font-weight: 600;
    }
    .boss-info a:hover {
      text-decoration: underline;
    }

    /* Back Button */
    .back-btn {
      background: #e2edf8;
      color: #286cdb;
      border: none;
      border-radius: 6px;
      padding: 8px 20px;
      cursor: pointer;
      font-size: 16px;
      margin-bottom: 24px;
      transition: background 0.18s ease;
    }
    .back-btn:hover {
      background: #bad8fd;
    }

        @media (max-width: 640px) {
      .courses-list {
        flex-direction: column;
        gap: 22px;
      }
      .about-boss {
        flex-direction: column;
        text-align: center;
      }
      .boss-info a {
        display: inline-block;
        margin-top: 8px;
      }
      .boss-photo {
        margin: 0 auto 12px;
      }
    }

</style>

</head>
<body>
<div class="name">
  <h1 class="gradient-text">Future Fly Tech</h1>
  <img src="C:\Users\DELL\Desktop\course app\futurelogo.jpg">
</div>
  <div class="container">
    <h1>Online Course Platform</h1>

    <h2>Categories</h2>
    <ul id="category-list" class="category-list"></ul>

    <h2>Courses</h2>
    <ul id="course-list" class="course-list"></ul>

  <section class="about-boss" aria-label="About the Boss">
      <img src="futurelogo.jpg" alt="Boss Photo" class="boss-photo" />
      <div class="boss-info">
        <h3>About the Boss</h3>
        <p><strong>Name:</strong> Mr. Abdul Samade</p>
        <p><strong>Position:</strong> Founder & CEO</p>
        <p><strong>Email:</strong> <a href="mailto:john.anderson@coursesapp.com">futureflytech@gmail.com <p>https://futureflyt.com</p></a></p>
        <p><strong>Bio:</strong> John is a seasoned professional with over 15 years in the e-learning industry, committed to providing quality education.</p>
      </div>
    </section>

  </div>

  <script src="app.js"></script>
  <script>
  // Mock data simulating what the backend might provide

const categories = [
  { id: '1', name: 'Aviation' },
  { id: '2', name: 'Digital Marketing' },
  { id: '3', name: 'Artificial Intelligence' }
];

const courses = [
  {
    id: '101',
    title: 'Introduction to Aviation',
    categoryId: '1',
    description: 'Learn the basics of aviation, aircraft types, and flight regulations.',
    videoUrl: 'aviation.v.mp4', // sample video
    instructor: 'Abdul Samade'
  },
  {
    id: '102',
    title: 'Digital Marketing Essentials',
    categoryId: '2',
    description: 'Master SEO, social media, and content marketing fundamentals.',
    videoUrl: 'dm.v.mp4',
    instructor: 'Abdul Samade'
  },
  {
    id: '103',
    title: 'AI for Beginners',
    categoryId: '3',
    description: 'Start your journey in Artificial Intelligence and Machine Learning.',
    videoUrl: 'ai.v.mp4',
    instructor: 'Abdul Samade'
  },
  {
    id: '104',
    title: 'Advanced AI Techniques',
    categoryId: '3',
    description: 'Deep dive into neural networks and deep learning architectures.',
    videoUrl: '',
    instructor: 'Abdul Samade'
  }
];

// DOM references
const categoryList = document.getElementById('category-list');
const courseList = document.getElementById('course-list');

let activeCategory = categories[0].id;

// Render categories
function renderCategories() {
  categoryList.innerHTML = '';
  categories.forEach(cat => {
    const li = document.createElement('li');
    li.textContent = cat.name;
    li.dataset.id = cat.id;
    if (cat.id === activeCategory) {
      li.classList.add('active');
    }
    li.addEventListener('click', () => {
      activeCategory = cat.id;
      renderCategories();
      renderCourses();
    });
    categoryList.appendChild(li);
  });
}

// Render courses filtered by active category
function renderCourses() {
  courseList.innerHTML = '';
  const filteredCourses = courses.filter(c => c.categoryId === activeCategory);
  if (filteredCourses.length === 0) {
    courseList.innerHTML = '<p>No courses in this category.</p>';
    return;
  }

  filteredCourses.forEach(course => {
    const li = document.createElement('li');

    const title = document.createElement('h3');
    title.className = 'course-title';
    title.textContent = course.title;

    const desc = document.createElement('p');
    desc.className = 'course-description';
    desc.textContent = course.description;

    li.appendChild(title);
    li.appendChild(desc);

    if (course.videoUrl) {
      const video = document.createElement ('video');
      video.className = 'video';
      video.controls = true;
      video.src = course.videoUrl;
      li.appendChild(video);
    }

    const instructor = document.createElement('p');
    instructor.className = 'instructor';
    instructor.textContent = `Instructor: ${course.instructor}`;
    li.appendChild(instructor);

    courseList.appendChild(li);
  });
}

// Initial rendering
renderCategories();
renderCourses();

</script>

</body>
</html>
