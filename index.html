// cursor
  const cur = document.getElementById('cursor');
  const ring = document.getElementById('cursorRing');
  let mx=0,my=0,rx=0,ry=0;
  document.addEventListener('mousemove',e=>{mx=e.clientX;my=e.clientY;cur.style.left=mx+'px';cur.style.top=my+'px';});
  (function animR(){rx+=(mx-rx)*.12;ry+=(my-ry)*.12;ring.style.left=rx+'px';ring.style.top=ry+'px';requestAnimationFrame(animR);})();
  document.querySelectorAll('a,button').forEach(el=>{
    el.addEventListener('mouseenter',()=>{cur.style.width='18px';cur.style.height='18px';ring.style.width='54px';ring.style.height='54px';});
    el.addEventListener('mouseleave',()=>{cur.style.width='10px';cur.style.height='10px';ring.style.width='36px';ring.style.height='36px';});
  });

  // smooth scroll
  document.querySelectorAll('a[href^="#"]').forEach(a=>{
    a.addEventListener('click',e=>{e.preventDefault();document.querySelector(a.getAttribute('href'))?.scrollIntoView({behavior:'smooth'});});
  });

  // scroll reveal
  const obs=new IntersectionObserver(entries=>{entries.forEach(en=>{if(en.isIntersecting){en.target.classList.add('visible');obs.unobserve(en.target);}});},{threshold:.1});
  document.querySelectorAll('.reveal,.work-card').forEach(el=>obs.observe(el));

  // skill bars
  const sbObs=new IntersectionObserver(entries=>{entries.forEach(en=>{if(en.isIntersecting){en.target.querySelectorAll('.skill-fill').forEach(f=>{f.style.width=f.dataset.w+'%';});sbObs.unobserve(en.target);}});},{threshold:.3});
  document.querySelectorAll('.skills-block').forEach(el=>sbObs.observe(el));

  // clock — WAT = UTC+1
  const sched=[
    {s:0,   e:8,    a:'😴 Fast asleep',           b:'Come back in the morning!'},
    {s:8,   e:11,   a:'🌅 Just woke up',           b:'Morning routine — might reply slowly'},
    {s:11,  e:12.5, a:'🧹 Doing house chores',     b:'Hands full — will reply soon'},
    {s:12.5,e:13.5, a:'💪 At the gym',             b:'Getting gains — check back at 2PM'},
    {s:13.5,e:14,   a:'🍽️ Having lunch',           b:'Eating right now — brb!'},
    {s:14,  e:20,   a:'💻 On the laptop — coding', b:'✅ Best time to reach me! Open to collabs.'},
    {s:20,  e:24,   a:'🌙 Evening wind-down',      b:'Relaxing — might still reply'},
  ];

  function getWAT(){const n=new Date();return new Date(n.getTime()+n.getTimezoneOffset()*60000+3600000);}
  function pad(n){return String(n).padStart(2,'0');}

  function tick(){
    const t=getWAT();
    const h=t.getHours(),m=t.getMinutes(),s=t.getSeconds();
    const ampm=h>=12?'PM':'AM',h12=h%12||12;
    document.getElementById('cDig').textContent=`${pad(h12)}:${pad(m)}:${pad(s)} ${ampm}`;
    const days=['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
    const months=['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
    document.getElementById('cDt').textContent=`${days[t.getDay()]} ${months[t.getMonth()]} ${t.getDate()} ${t.getFullYear()}`;
    document.getElementById('hS').style.transform=`rotate(${s*6}deg)`;
    document.getElementById('hM').style.transform=`rotate(${m*6+s*.1}deg)`;
    document.getElementById('hH').style.transform=`rotate(${(h%12)*30+m*.5}deg)`;
    const dec=h+m/60;
    const cur2=sched.find(x=>dec>=x.s&&dec<x.e)||sched[0];
    document.getElementById('snAct').textContent=cur2.a;
    document.getElementById('snSub').textContent=cur2.b;
    document.querySelectorAll('.sched-row').forEach(row=>{
      const rs=parseFloat(row.dataset.s),re=parseFloat(row.dataset.e),on=dec>=rs&&dec<re;
      row.classList.toggle('sa-row',on);
      row.querySelector('.s-dot').classList.toggle('sa',on);
      row.querySelector('.s-lbl').classList.toggle('sa',on);
      row.querySelector('.s-time').classList.toggle('sa',on);
    });
  }
  tick();setInterval(tick,1000);

  // story accordion
  function toggleStory(btn){
    const body=btn.nextElementSibling;
    const arr=btn.querySelector('.story-arr');
    const open=body.classList.contains('open');
    document.querySelectorAll('.story-body.open').forEach(b=>{b.classList.remove('open');b.previousElementSibling.querySelector('.story-arr').textContent='+';});
    if(!open){body.classList.add('open');arr.textContent='−';}
  }
