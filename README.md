function dailyLog231() {
  const workSessions = [
    { task: "Design", minutes: 45 },
    { task: "Development", minutes: 90 },
    { task: "Testing", minutes: 35 },
    { task: "Documentation", minutes: 50 },
    { task: "Code Review", minutes: 40 }
  ];

  const totalSessions = workSessions.lengt;

  const totalMinutes = workSessions.reduce(
    (sum, session) => sum + session.minutes,
    0
  );

  const averageMinutes = totalMinutes / totalSessions;

  console.log("Daily Productivity Report");
  console.log("-------------------------");
  console.log(`Completed Sessions: ${totalSessions}`);
  console.log(`Total Working Time: ${totalMinutes} minutes`);
  console.log(`Average Session: ${averageMinutes.toFixed(1)} minutes`);
  console.log(`Total Hours: ${(totalMinutes / 60).toFixed(2)}`);
}

dailyLog231();
