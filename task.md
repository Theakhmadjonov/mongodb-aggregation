use school

## Ma'lumotlar bazasi tuzilishi

db.createCollection("students")
db.createCollection("subjects")
db.createCollection("teachers")
db.createCollection("grades")
db.createCollection("attendance")

### 1. `students` (O'quvchilar)

<!-- db.students.insertMany([
{
"_id": ObjectId("5f8a776c1234567890123456"),
"student_id": "ST001",
"full_name": "Alisher Qodirov",
"grade": "9-A",
"birth_date": ISODate("2008-05-12T00:00:00Z"),
"address": {
"district": "Yunusobod",
"street": "Amir Temur"
},
"contact": {
"phone": "+998901234567",
"email": "alisher@example.com"
},
"enrolled_date": ISODate("2022-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c1234567890123457"),
"student_id": "ST002",
"full_name": "Gulnora Rahimova",
"grade": "8-B",
"birth_date": ISODate("2009-02-28T00:00:00Z"),
"address": {
"district": "Mirzo Ulugbek",
"street": "Mustaqillik"
},
"contact": {
"phone": "+998901234568",
"email": "gulnora@example.com"
},
"enrolled_date": ISODate("2022-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c1234567890123458"),
"student_id": "ST003",
"full_name": "Bobur Karimov",
"grade": "10-A",
"birth_date": ISODate("2007-11-15T00:00:00Z"),
"address": {
"district": "Chilonzor",
"street": "Bunyodkor"
},
"contact": {
"phone": "+998901234569",
"email": "bobur@example.com"
},
"enrolled_date": ISODate("2021-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c1234567890123459"),
"student_id": "ST004",
"full_name": "Madina Toshpulatova",
"grade": "9-B",
"birth_date": ISODate("2008-06-20T00:00:00Z"),
"address": {
"district": "Yashnobod",
"street": "Istiqlol"
},
"contact": {
"phone": "+998901234570",
"email": "madina@example.com"
},
"enrolled_date": ISODate("2022-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c123456789012345a"),
"student_id": "ST005",
"full_name": "Sardor Jorayev",
"grade": "11-A",
"birth_date": ISODate("2006-09-05T00:00:00Z"),
"address": {
"district": "Shayxontohur",
"street": "Navoiy"
},
"contact": {
"phone": "+998901234571",
"email": "sardor@example.com"
},
"enrolled_date": ISODate("2020-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c123456789012345b"),
"student_id": "ST006",
"full_name": "Aziza Normatova",
"grade": "9-A",
"birth_date": ISODate("2008-07-25T00:00:00Z"),
"address": {
"district": "Yunusobod",
"street": "Bog'ishamol"
},
"contact": {
"phone": "+998901234572",
"email": "aziza@example.com"
},
"enrolled_date": ISODate("2022-09-01T00:00:00Z")
},
{
"_id": ObjectId("5f8a776c123456789012345c"),
"student_id": "ST007",
"full_name": "Dilshod Olimov",
"grade": "10-A",
"birth_date": ISODate("2007-03-15T00:00:00Z"),
"address": {
"district": "Chilonzor",
"street": "Muhabbat"
},
"contact": {
"phone": "+998901234573",
"email": "dilshod@example.com"
},
"enrolled_date": ISODate("2021-09-01T00:00:00Z")
}
]) -->

### 2. `subjects` (Fanlar)

<!-- db.subjects.insertMany([
{
"\_id": ObjectId("5f8a776c123456789012345d"),
"subject_id": "SUB001",
"name": "Matematika",
"category": "Aniq fanlar",
"hours_per_week": 6,
"required_materials": ["Darslik", "Masalalar to'plami", "Kalkulyator"]
},
{
"\_id": ObjectId("5f8a776c123456789012345e"),
"subject_id": "SUB002",
"name": "Fizika",
"category": "Aniq fanlar",
"hours_per_week": 4,
"required_materials": ["Darslik", "Laboratoriya jihozlari"]
},
{
"\_id": ObjectId("5f8a776c123456789012345f"),
"subject_id": "SUB003",
"name": "Informatika",
"category": "Aniq fanlar",
"hours_per_week": 4,
"required_materials": ["Darslik", "Kompyuter", "Dasturlash muhiti"]
},
{
"\_id": ObjectId("5f8a776c1234567890123460"),
"subject_id": "SUB004",
"name": "Ingliz tili",
"category": "Chet tillari",
"hours_per_week": 5,
"required_materials": ["Darslik", "Lug'at", "Audio materiallar"]
},
{
"\_id": ObjectId("5f8a776c1234567890123461"),
"subject_id": "SUB005",
"name": "Biologiya",
"category": "Tabiiy fanlar",
"hours_per_week": 3,
"required_materials": ["Darslik", "Laboratoriya jihozlari"]
},
{
"\_id": ObjectId("5f8a776c1234567890123462"),
"subject_id": "SUB006",
"name": "Tarix",
"category": "Ijtimoiy fanlar",
"hours_per_week": 3,
"required_materials": ["Darslik", "Tarixiy xaritalar"]
}
]) -->

### 3. `teachers` (O'qituvchilar)

<!-- db.teachers.insertMany([
{
"\_id": ObjectId("5f8a776c1234567890123463"),
"teacher_id": "TCH001",
"full_name": "Karimov Botir",
"subjects": ["SUB001"],
"experience_years": 15,
"hire_date": ISODate("2010-08-15T00:00:00Z"),
"contact": {
"phone": "+998901234580",
"email": "karimov@example.com"
},
"education": "Oliy toifali o'qituvchi"
},
{
"\_id": ObjectId("5f8a776c1234567890123464"),
"teacher_id": "TCH002",
"full_name": "Alimova Nilufar",
"subjects": ["SUB002"],
"experience_years": 10,
"hire_date": ISODate("2015-08-20T00:00:00Z"),
"contact": {
"phone": "+998901234581",
"email": "alimova@example.com"
},
"education": "1-toifali o'qituvchi"
},
{
"\_id": ObjectId("5f8a776c1234567890123465"),
"teacher_id": "TCH003",
"full_name": "Usmonov Javohir",
"subjects": ["SUB003"],
"experience_years": 8,
"hire_date": ISODate("2017-08-25T00:00:00Z"),
"contact": {
"phone": "+998901234582",
"email": "usmonov@example.com"
},
"education": "2-toifali o'qituvchi"
},
{
"\_id": ObjectId("5f8a776c1234567890123466"),
"teacher_id": "TCH004",
"full_name": "Smith John",
"subjects": ["SUB004"],
"experience_years": 12,
"hire_date": ISODate("2013-08-15T00:00:00Z"),
"contact": {
"phone": "+998901234583",
"email": "smith@example.com"
},
"education": "Oliy toifali o'qituvchi"
},
{
"\_id": ObjectId("5f8a776c1234567890123467"),
"teacher_id": "TCH005",
"full_name": "Karimova Sevara",
"subjects": ["SUB005"],
"experience_years": 7,
"hire_date": ISODate("2018-08-20T00:00:00Z"),
"contact": {
"phone": "+998901234584",
"email": "karimova@example.com"
},
"education": "2-toifali o'qituvchi"
},
{
"\_id": ObjectId("5f8a776c1234567890123468"),
"teacher_id": "TCH006",
"full_name": "Mahmudov Akbar",
"subjects": ["SUB006"],
"experience_years": 20,
"hire_date": ISODate("2005-08-15T00:00:00Z"),
"contact": {
"phone": "+998901234585",
"email": "mahmudov@example.com"
},
"education": "Oliy toifali o'qituvchi"
}
]) -->

### 4. `grades` (Baholar)

<!-- db.grades.insertMany([
{
"\_id": ObjectId("5f8a776c1234567890123469"),
"student_id": "ST001",
"subject_id": "SUB001",
"teacher_id": "TCH001",
"grades": [5, 4, 5, 4, 5],
"average_grade": 4.6,
"semester": "Kuz-2023",
"test_scores": [92, 88, 95]
},
{
"\_id": ObjectId("5f8a776c123456789012346a"),
"student_id": "ST001",
"subject_id": "SUB002",
"teacher_id": "TCH002",
"grades": [4, 5, 4, 4],
"average_grade": 4.25,
"semester": "Kuz-2023",
"test_scores": [85, 90, 82]
},
{
"\_id": ObjectId("5f8a776c123456789012346b"),
"student_id": "ST001",
"subject_id": "SUB003",
"teacher_id": "TCH003",
"grades": [5, 5, 5, 4, 5],
"average_grade": 4.8,
"semester": "Kuz-2023",
"test_scores": [98, 95, 97]
},
{
"\_id": ObjectId("5f8a776c123456789012346c"),
"student_id": "ST002",
"subject_id": "SUB004",
"teacher_id": "TCH004",
"grades": [4, 4, 5, 4],
"average_grade": 4.25,
"semester": "Kuz-2023",
"test_scores": [82, 86, 85]
},
{
"\_id": ObjectId("5f8a776c123456789012346d"),
"student_id": "ST002",
"subject_id": "SUB006",
"teacher_id": "TCH006",
"grades": [5, 5, 5, 5],
"average_grade": 5.0,
"semester": "Kuz-2023",
"test_scores": [96, 98, 97]
},
{
"\_id": ObjectId("5f8a776c123456789012346e"),
"student_id": "ST003",
"subject_id": "SUB001",
"teacher_id": "TCH001",
"grades": [4, 3, 4, 4],
"average_grade": 3.75,
"semester": "Kuz-2023",
"test_scores": [75, 70, 78]
},
{
"\_id": ObjectId("5f8a776c123456789012346f"),
"student_id": "ST003",
"subject_id": "SUB005",
"teacher_id": "TCH005",
"grades": [5, 5, 5, 4, 5],
"average_grade": 4.8,
"semester": "Kuz-2023",
"test_scores": [94, 92, 95]
},
{
"\_id": ObjectId("5f8a776c1234567890123470"),
"student_id": "ST004",
"subject_id": "SUB002",
"teacher_id": "TCH002",
"grades": [3, 4, 3, 3],
"average_grade": 3.25,
"semester": "Kuz-2023",
"test_scores": [65, 70, 68]
},
{
"\_id": ObjectId("5f8a776c1234567890123471"),
"student_id": "ST004",
"subject_id": "SUB004",
"teacher_id": "TCH004",
"grades": [5, 5, 5, 4, 5],
"average_grade": 4.8,
"semester": "Kuz-2023",
"test_scores": [92, 95, 94]
},
{
"\_id": ObjectId("5f8a776c1234567890123472"),
"student_id": "ST005",
"subject_id": "SUB001",
"teacher_id": "TCH001",
"grades": [5, 5, 5, 5],
"average_grade": 5.0,
"semester": "Kuz-2023",
"test_scores": [98, 100, 97]
},
{
"\_id": ObjectId("5f8a776c1234567890123473"),
"student_id": "ST005",
"subject_id": "SUB003",
"teacher_id": "TCH003",
"grades": [5, 5, 5, 5],
"average_grade": 5.0,
"semester": "Kuz-2023",
"test_scores": [100, 98, 99]
},
{
"\_id": ObjectId("5f8a776c1234567890123474"),
"student_id": "ST006",
"subject_id": "SUB001",
"teacher_id": "TCH001",
"grades": [4, 4, 5, 4],
"average_grade": 4.25,
"semester": "Kuz-2023",
"test_scores": [85, 82, 88]
},
{
"\_id": ObjectId("5f8a776c1234567890123475"),
"student_id": "ST006",
"subject_id": "SUB002",
"teacher_id": "TCH002",
"grades": [5, 4, 5, 4],
"average_grade": 4.5,
"semester": "Kuz-2023",
"test_scores": [88, 92, 90]
},
{
"\_id": ObjectId("5f8a776c1234567890123476"),
"student_id": "ST007",
"subject_id": "SUB005",
"teacher_id": "TCH005",
"grades": [4, 3, 4, 4],
"average_grade": 3.75,
"semester": "Kuz-2023",
"test_scores": [76, 72, 78]
},
{
"\_id": ObjectId("5f8a776c1234567890123477"),
"student_id": "ST007",
"subject_id": "SUB006",
"teacher_id": "TCH006",
"grades": [5, 4, 5, 5],
"average_grade": 4.75,
"semester": "Kuz-2023",
"test_scores": [92, 90, 95]
}
]) -->

### 5. `attendance` (Davomatlar)

<!-- db.attendance.insertMany([
{
"_id": ObjectId("5f8a776c1234567890123478"),
"student_id": "ST001",
"subject_id": "SUB001",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c1234567890123479"),
"student_id": "ST001",
"subject_id": "SUB002",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c123456789012347a"),
"student_id": "ST002",
"subject_id": "SUB004",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "absent",
"note": "Kasal"
},
{
"_id": ObjectId("5f8a776c123456789012347b"),
"student_id": "ST003",
"subject_id": "SUB001",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c123456789012347c"),
"student_id": "ST004",
"subject_id": "SUB002",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "late",
"note": "10 daqiqa kech qoldi"
},
{
"_id": ObjectId("5f8a776c123456789012347d"),
"student_id": "ST005",
"subject_id": "SUB003",
"date": ISODate("2023-11-01T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c123456789012347e"),
"student_id": "ST001",
"subject_id": "SUB001",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c123456789012347f"),
"student_id": "ST002",
"subject_id": "SUB006",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "absent",
"note": "Kasal"
},
{
"_id": ObjectId("5f8a776c1234567890123480"),
"student_id": "ST003",
"subject_id": "SUB005",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c1234567890123481"),
"student_id": "ST004",
"subject_id": "SUB004",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c1234567890123482"),
"student_id": "ST005",
"subject_id": "SUB001",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c1234567890123483"),
"student_id": "ST006",
"subject_id": "SUB001",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "present",
"note": ""
},
{
"_id": ObjectId("5f8a776c1234567890123484"),
"student_id": "ST006",
"subject_id": "SUB002",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "absent",
"note": "Sababsiz"
},
{
"_id": ObjectId("5f8a776c1234567890123485"),
"student_id": "ST007",
"subject_id": "SUB005",
"date": ISODate("2023-11-02T00:00:00Z"),
"status": "late",
"note": "5 daqiqa kech qoldi"
}
]) -->

### Topshiriq 1: $group operatori bilan o'quvchilarni sinflarga guruhlash

<!-- db.students.aggregate([
  {
    $group: {
      _id: "$grade",
      total_students: { $sum: 1 }
    }
  },
  {
    $sort: { total_students: -1 }
  }
]) -->

### Topshiriq 2: $group va accumulator operatorlari

<!-- db.grades.aggregate([
  {
    $group: {
      _id: "$subject_id",
      average_grade: { $avg: "$average_grade" }
    }
  },
  {
    $sort: { average_grade: -1 }
  },
  {
    $lookup: {
      from: "subjects",
      localField: "_id",
      foreignField: "subject_id",
      as: "subject_info"
    }
  },
  {
    $project: {
      _id: 0,
      subject_name: { $arrayElemAt: ["$subject_info.name", 0] },
      average_grade: 1
    }
  }
]) -->

### Topshiriq 3: $lookup bilan o'quvchilar va baholari

<!-- db.students.aggregate([
  {
    $lookup: {
      from: "grades",
      localField: "student_id",
      foreignField: "student_id",
      as: "grades_info"
    }
  },
  {
    $unwind: "$grades_info"
  },
  {
    $project: {
      full_name: 1,
      grade: 1,
      grades: "$grades_info.grades",
      subject: "$grades_info.subject_id",
      average_grade: "$grades_info.average_grade"
    }
  }
]) -->

### Topshiriq 4: $lookup bilan o'qituvchilar va fanlar

<!-- db.teachers.aggregate([
  {
    $lookup: {
      from: "subjects",
      localField: "subjects",
      foreignField: "subject_id",
      as: "teacher_subjects"
    }
  },
  {
    $project: {
      _id: 0,
      full_name: 1,
      experience_years: 1,
      teacher_subjects: {
        name: 1,
        category: 1,
        hours_per_week: 1,
        required_materials: 1
      }
    }
  }
]); -->

### Topshiriq 5: $group va $lookup kombinatsiyasi

<!-- db.students.aggregate([
  {
    $lookup: {
      from: "grades",
      localField: "student_id",
      foreignField: "student_id",
      as: "grades_info"
    }
  },
  {
    $unwind: "$grades_info"
  },
  {
    $lookup: {
      from: "subjects",
      localField: "grades_info.subject_id",
      foreignField: "subject_id",
      as: "subject_info"
    }
  },
  {
    $unwind: "$subject_info"
  },
  {
    $group: {
      _id: "$grade",
      average_grade: { $avg: "$grades_info.average_grade" }
    }
  },
  {
    $sort: { _id: 1 }
  }
]); -->

### Topshiriq 6: Davomat va baholar analitikasi

<!-- db.attendance.aggregate([
  {
    $lookup: {
      from: "grades",
      localField: "student_id",
      foreignField: "student_id",
      as: "grades_info"
    }
  },
  {
    $unwind: "$grades_info"
  },
  {
    $group: {
      _id: {
        student_id: "$student_id",
        status: "$status"
      },
      average_grade: { $avg: "$grades_info.average_grade" }
    }
  },
  {
    $group: {
      _id: "$_id.status",
      avg_grade: { $avg: "$average_grade" }
    }
  },
  {
    $sort: { _id: 1 }
  }
]); -->

### Topshiriq 7: Fanlar kategoriyasi bo'yicha analitika

<!-- db.subjects.aggregate([
  {
    $lookup: {
      from: "grades",
      localField: "subject_id",
      foreignField: "subject_id",
      as: "subject_grades"
    }
  },
  {
    $group: {
      _id: "$category",
      total_subjects: { $sum: 1 },
      avg_hours_per_week: { $avg: "$hours_per_week" },
      avg_grade: {
        $avg: {
          $avg: "$subject_grades.average_grade"
        }
      }
    }
  },
  {
    $sort: { _id: 1 }
  }
]) -->
