<template>
  <div class="school-intro">
    <header class="header">
      <h1 class="title">清远市博爱学校</h1>
      <p class="subtitle">博爱 · 博学 · 博大 | 成立于1998年</p>
    </header>
    
    <div class="content-grid">
      <div class="card blue-card animated">
        <h2 class="card-title"><i class="fas fa-school"></i> 学校概况</h2>
        <div class="card-content">
          <p>清远市博爱学校成立于1998年，是由清远市红十字会创办的一所大型现代化民办学校，集幼儿园、小学、初中和高中于一体。</p>
          <p>学校位于广东清远市，地处市政府旁、北江河畔城市中轴线。现有校园用地面积65亩（新校区规划建设用地200亩），办学规模近100个教学班，约4500名学生。</p>
        </div>
      </div>
      
      <div class="card green-card animated delay-1">
        <h2 class="card-title"><i class="fas fa-user-tie"></i> 领导团队</h2>
        <div class="card-content">
          <p><strong>现任校长：</strong>马正军</p>
          <p><strong>校训：</strong>博爱、博学和博大</p>
          <p><strong>办学理念：</strong>"以师为本、学生为重"</p>
          <p><strong>红会精神：</strong>弘扬"人道、博爱、奉献"的红十字精神</p>
        </div>
      </div>
      
      <div class="card orange-card animated delay-2">
        <h2 class="card-title"><i class="fas fa-trophy"></i> 学校荣誉</h2>
        <div class="card-content">
          <p>2010年，学校荣获"清远市清城区科普特色学校"和"清城区德育示范学校"称号</p>
          <p>被广东省红十字会评为"广东省红十字青少年示范学校"的先进单位</p>
          <p>2008年成为全市首家通过"广东省义务教育规范化学校"评估验收的民办学校</p>
          <p>2004年被市政府确定为"市中心区域优质学校"</p>
        </div>
      </div>
    </div>
    
    <div class="highlight">
      <h2 class="highlight-title">新校区发展里程碑</h2>
      <div class="content-grid">
        <div class="card image-card animated" :style="{ backgroundImage: 'url(https://images.unsplash.com/photo-1523050854058-8df90110c9f1?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80)' }">
          <div class="card-overlay"></div>
          <div class="card-content">
            <div class="achievement">
              <div class="achievement-year">2020年9月1日</div>
              <p>新校区启用，设为中学部，旧校区仍为小学部</p>
            </div>
          </div>
        </div>
        
        <div class="card image-card animated delay-1" :style="{ backgroundImage: 'url(https://images.unsplash.com/photo-1541339907198-e08756dedf3f?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80)' }">
          <div class="card-overlay"></div>
          <div class="card-content">
            <div class="achievement">
              <div class="achievement-year">2021年12月26日</div>
              <p>学校成为华师附中在清远授牌的唯一"优质生源基地"</p>
            </div>
          </div>
        </div>
        
        <div class="card image-card animated delay-2" :style="{ backgroundImage: 'url(https://images.unsplash.com/photo-1523580494863-6f3031224c94?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80)' }">
          <div class="card-overlay"></div>
          <div class="card-content">
            <div class="achievement">
              <div class="achievement-year">2025年</div>
              <p>与华南师大附中联合创办"博爱・华附海航少年班"，旨在培养热爱海空、适合飞行、素质全面的精英苗子</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="stats-container">
      <div class="stat-box blue-bg animated">
        <span class="stat-number">{{ teacherCount }}</span>
        <div class="stat-label">教师人数</div>
      </div>
      
      <div class="stat-box green-bg animated delay-1">
        <span class="stat-number">{{ formalTeachers }}</span>
        <div class="stat-label">事业编制教师</div>
      </div>
      
      <div class="stat-box orange-bg animated delay-2">
        <span class="stat-number">{{ seniorTeachers }}%</span>
        <div class="stat-label">高级教师占比</div>
      </div>
      
      <div class="stat-box purple-bg animated delay-3">
        <span class="stat-number">{{ experiencedTeachers }}%</span>
        <div class="stat-label">5年以上教龄教师</div>
      </div>
    </div>
    
    <div class="content-grid">
      <div class="card blue-card animated">
        <h2 class="card-title"><i class="fas fa-chalkboard-teacher"></i> 师资力量</h2>
        <div class="card-content">
          <p>学校现有教师200余人，其中事业编制教师90人，教师队伍的年龄结构、性别结构、地域结构、学历结构、专业结构、职称结构合理。</p>
          <p>教师学历百分之百达标，硕士研究生3人，高级教师占教师总数的65%，每学年教师流动率控制在5%以内。幼儿园和小学部校龄5年以上的教师占75%。</p>
        </div>
      </div>
      
      <div class="card image-card animated delay-1" :style="{ backgroundImage: 'url(https://images.unsplash.com/photo-1523050854058-8df90110c9f1?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80)' }">
        <div class="card-overlay"></div>
        <div class="card-content">
          <h2 class="card-title"><i class="fas fa-building"></i> 学校环境</h2>
          <p>学校按省一级学校的标准设置建设，各项硬件设施配备先进齐全：</p>
          <ul class="feature-list">
            <li><i class="fas fa-check"></i> 30多间功能专用室</li>
            <li><i class="fas fa-check"></i> 多媒体校园网、闭路电视网和立体声广播通讯系统</li>
            <li><i class="fas fa-check"></i> 8~10人一间的学生宿舍，配有电话、空调等设施</li>
            <li><i class="fas fa-check"></i> 200米标准运动场、篮球场、足球场等体育设施</li>
          </ul>
        </div>
      </div>
    </div>
    
    <div class="card purple-card animated">
      <h2 class="card-title"><i class="fas fa-star"></i> 教学特色</h2>
      <div class="card-content">
        <p>学校实施多元化的教学特色：</p>
        <ul class="feature-list">
          <li><i class="fas fa-graduation-cap"></i> 外教英语、分层教学</li>
          <li><i class="fas fa-graduation-cap"></i> 科技创新活动、红十字青少年活动</li>
          <li><i class="fas fa-graduation-cap"></i> 孝敬教育、阳光体育、艺术教育</li>
          <li><i class="fas fa-graduation-cap"></i> 初中"三质"（素质、体质、气质）教育</li>
          <li><i class="fas fa-graduation-cap"></i> 高中"四自"（自信、自立、自律、自强）教育</li>
          <li><i class="fas fa-graduation-cap"></i> "十维度四等级"学生综合素质评价体系</li>
        </ul>
      </div>
    </div>
    
    <div class="motto blue-card animated">
      "以师为本、学生为重" - 遵循国家教育方针，注重学生综合素质和实验能力的培养，为社会主义建设事业培育仁厚睿智、学识渊博、志向远大的接班人。
    </div>
    
    <div class="card orange-card animated">
      <h2 class="card-title"><i class="fas fa-medal"></i> 办学成绩</h2>
      <div class="card-content">
        <div class="achievement">
          <div class="achievement-year">2009-2016年</div>
          <p>连续八届中考"清远市第一中学正取上线率"、"考生总平均分"等多项主要指标获得市中心区域"八连冠"</p>
        </div>
        
        <div class="achievement">
          <div class="achievement-year">2014年</div>
          <p>首届高考"开门红"！63名考生重本7人、本A以上29人、本B以上41人，本科上线率65.08%</p>
        </div>
        
        <div class="achievement">
          <div class="achievement-year">2025年</div>
          <p>高考实现了从0到1的突破！陈国臣同学考进清华大学！</p>
        </div>
        
        <p>高中部实行"高考目标承诺制"办学首开全国先河，以中考成绩承诺高考目标（分五等：985院校、211大学、普通重本、本A、本B）。高中阶段三年学杂费在高考目标兑现后一次性缴纳，未能兑现的免收高中阶段三年学杂费。</p>
      </div>
    </div>
    
    <footer class="footer green-card animated">
      <p>清远市博爱学校 © 2023 | 博爱 · 博学 · 博大</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'SchoolIntroduction',
  data() {
    return {
      teacherCount: 200,
      formalTeachers: 90,
      seniorTeachers: 65,
      experiencedTeachers: 75
    }
  },
  mounted() {
    this.animateNumbers();
    this.setupScrollAnimations();
  },
  methods: {
    animateNumbers() {
      const stats = [
        { element: this.$el.querySelector('.stat-number:nth-child(1)'), target: this.teacherCount },
        { element: this.$el.querySelector('.stat-number:nth-child(2)'), target: this.formalTeachers },
        { element: this.$el.querySelector('.stat-number:nth-child(3)'), target: this.seniorTeachers },
        { element: this.$el.querySelector('.stat-number:nth-child(4)'), target: this.experiencedTeachers }
      ];
      
      stats.forEach(stat => {
        let current = 0;
        const duration = 2000;
        const steps = 50;
        const increment = stat.target / steps;
        const stepTime = duration / steps;
        
        const timer = setInterval(() => {
          current += increment;
          if (current >= stat.target) {
            clearInterval(timer);
            current = stat.target;
          }
          stat.element.textContent = Math.round(current);
        }, stepTime);
      });
    },
    setupScrollAnimations() {
      const animatedElements = this.$el.querySelectorAll('.animated');
      
      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.style.visibility = 'visible';
            entry.target.style.animationPlayState = 'running';
            observer.unobserve(entry.target);
          }
        });
      }, { threshold: 0.1 });
      
      animatedElements.forEach(element => {
        element.style.visibility = 'hidden';
        element.style.animationPlayState = 'paused';
        observer.observe(element);
      });
    }
  }
}
</script>

<style scoped>
.school-intro {
  max-width: 1200px;
  margin: 0 auto;
  padding: 30px 20px;
  font-family: 'Noto Sans SC', sans-serif;
  color: #333;
  line-height: 1.7;
}

.header {
  text-align: center;
  margin-bottom: 50px;
  padding: 40px 30px;
  background: linear-gradient(135deg, #3a86ff 0%, #5e60ce 100%);
  color: white;
  border-radius: 20px;
  box-shadow: 0 15px 30px -10px rgba(0, 0, 0, 0.15);
  position: relative;
  overflow: hidden;
}

.title {
  font-size: 3.2rem;
  font-weight: 700;
  margin-bottom: 15px;
  letter-spacing: 1px;
  position: relative;
  text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
}

.subtitle {
  font-size: 1.3rem;
  opacity: 0.9;
  font-weight: 300;
  max-width: 600px;
  margin: 0 auto;
}

.content-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 30px;
  margin-bottom: 40px;
}

.card {
  border-radius: 16px;
  box-shadow: 0 10px 20px -8px rgba(0, 0, 0, 0.12);
  padding: 30px;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  height: 100%;
  display: flex;
  flex-direction: column;
  position: relative;
  overflow: hidden;
}

.card:hover {
  transform: translateY(-8px);
  box-shadow: 0 15px 30px -10px rgba(0, 0, 0, 0.15);
}

.blue-card {
  background: linear-gradient(135deg, #3a86ff 0%, #5e60ce 100%);
  color: white;
}

.green-card {
  background: linear-gradient(135deg, #4ecdc4 0%, #44a08d 100%);
  color: white;
}

.orange-card {
  background: linear-gradient(135deg, #ff9a8b 0%, #ff6a88 100%);
  color: white;
}

.purple-card {
  background: linear-gradient(135deg, #a18cd1 0%, #fbc2eb 100%);
  color: white;
}

.image-card {
  background-size: cover;
  background-position: center;
  color: white;
  min-height: 280px;
}

.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(0, 0, 0, 0.6);
  z-index: 1;
}

.card-content {
  position: relative;
  z-index: 2;
  flex-grow: 1;
}

.card-content p {
  margin-bottom: 18px;
}

.card-title {
  font-size: 1.6rem;
  margin-bottom: 20px;
  display: flex;
  align-items: center;
  position: relative;
}

.card-title i {
  margin-right: 12px;
  font-size: 2rem;
}

.blue-card .card-title i,
.green-card .card-title i,
.orange-card .card-title i,
.purple-card .card-title i,
.image-card .card-title i {
  color: rgba(255, 255, 255, 0.9);
}

.highlight {
  margin: 40px 0;
  position: relative;
}

.highlight-title {
  text-align: center;
  margin-bottom: 30px;
  color: #212529;
  font-size: 2rem;
  font-weight: 600;
  position: relative;
  display: inline-block;
  left: 50%;
  transform: translateX(-50%);
  padding: 0 20px;
}

.highlight-title::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, #3a86ff 0%, #4ecdc4 100%);
  border-radius: 10px;
}

.stats-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 25px;
  margin: 40px 0;
}

.stat-box {
  text-align: center;
  padding: 30px 20px;
  border-radius: 16px;
  box-shadow: 0 10px 20px -8px rgba(0, 0, 0, 0.12);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  position: relative;
  overflow: hidden;
  color: white;
}

.stat-box:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px -10px rgba(0, 0, 0, 0.15);
}

.blue-bg {
  background: linear-gradient(135deg, #3a86ff 0%, #5e60ce 100%);
}

.green-bg {
  background: linear-gradient(135deg, #4ecdc4 0%, #44a08d 100%);
}

.orange-bg {
  background: linear-gradient(135deg, #ff9a8b 0%, #ff6a88 100%);
}

.purple-bg {
  background: linear-gradient(135deg, #a18cd1 0%, #fbc2eb 100%);
}

.stat-number {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 10px;
  display: block;
  text-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.stat-label {
  font-size: 1.1rem;
  font-weight: 500;
}

.feature-list {
  list-style-type: none;
  margin: 25px 0;
}

.feature-list li {
  padding: 12px 0;
  border-bottom: 1px solid rgba(255, 255, 255, 0.2);
  display: flex;
  align-items: center;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.feature-list li:hover {
  background-color: rgba(255, 255, 255, 0.1);
  padding-left: 10px;
  border-radius: 8px;
}

.feature-list li i {
  margin-right: 15px;
  font-size: 1.2rem;
  width: 25px;
  text-align: center;
}

.achievement {
  padding: 25px;
  border-radius: 16px;
  margin: 25px 0;
  box-shadow: 0 5px 15px -5px rgba(0, 0, 0, 0.08);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
}

.achievement:hover {
  transform: translateX(5px);
  box-shadow: 0 10px 20px -8px rgba(0, 0, 0, 0.12);
}

.achievement-year {
  font-weight: 700;
  margin-bottom: 12px;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
}

.achievement-year::before {
  content: '✓';
  margin-right: 10px;
  background: rgba(255, 255, 255, 0.9);
  color: #3a86ff;
  width: 24px;
  height: 24px;
  border-radius: 50%;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-size: 0.9rem;
}

.motto {
  text-align: center;
  font-style: italic;
  padding: 40px;
  border-radius: 20px;
  margin: 50px 0;
  font-size: 1.5rem;
  box-shadow: 0 10px 20px -8px rgba(0, 0, 0, 0.12);
  position: relative;
}

.footer {
  text-align: center;
  margin-top: 70px;
  padding: 30px;
  border-radius: 16px;
  box-shadow: 0 5px 15px -5px rgba(0, 0, 0, 0.08);
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.animated {
  animation: fadeIn 0.8s ease-out forwards;
}

.delay-1 { animation-delay: 0.2s; }
.delay-2 { animation-delay: 0.4s; }
.delay-3 { animation-delay: 0.6s; }

@media (max-width: 768px) {
  .content-grid {
    grid-template-columns: 1fr;
  }
  
  .title {
    font-size: 2.5rem;
  }
  
  .stats-container {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .header {
    padding: 30px 20px;
  }
  
  .motto {
    padding: 30px 20px;
    font-size: 1.3rem;
  }
}

@media (max-width: 480px) {
  .stats-container {
    grid-template-columns: 1fr;
  }
  
  .title {
    font-size: 2rem;
  }
  
  .card-title {
    font-size: 1.4rem;
  }
}
</style>