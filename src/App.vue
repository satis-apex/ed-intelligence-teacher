<template>
  <div id="app" class="theme-layout">
    <Header />
    <Subheader />
    <Mobilemenu />
    <router-view></router-view>
    <notifications group="notificationAlerts" />
    <Footer />
  </div>
</template>

<script>
import Header from './components/layout/header/Header.vue'
import Subheader from './components/layout/subheader/Subheader.vue'
import Mobilemenu from './components/navigation/mobilemenu/Mobilemenu.vue'
import Home from './pages/Home.vue'
import Admin from './pages/GoogleClassrom.vue'
import LessonPlanBank from './pages/LessonPlanBank.vue'
import AddStudent from './pages/AddStudent.vue'
import LessonPlanSingle from './pages/LessonPlanSingle.vue'
import ChangePassword from './pages/ChangePassword.vue'
import ProfileSettings from './pages/ProfileSettings.vue'
import NotificationsTable from './pages/NotificationsTable.vue'
import LessonPlan from './pages/LessonPlan.vue'
import Footer from './components/layout/footer/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Subheader,
    Mobilemenu,
    Home,
    Admin,
    LessonPlanBank,
    LessonPlanSingle,
    AddStudent,
    LessonPlan,
    NotificationsTable,
    ChangePassword,
    ProfileSettings,
    Footer
  },
  data() {
    return {
      showWhich: "Home"
    }
  }
}
</script>