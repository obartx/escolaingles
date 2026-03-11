import React, { useState, useEffect } from 'react';
import { 
  Globe, ShieldCheck, UserPlus, LogIn, 
  ChevronRight, BookOpen, GraduationCap, 
  LayoutDashboard, Users, Settings, LogOut,
  CheckCircle2, AlertCircle, FileText, PlayCircle,
  Clock, Award, Calendar
} from 'lucide-react';

const App = () => {
  const [page, setPage] = useState('landing'); 
  const [user, setUser] = useState(null);
  const [email, setEmail] = useState('');
  const [password, setPassword] = useState('');
  const [regName, setRegName] = useState('');
  const [regEmail, setRegEmail] = useState('');
  const [regPass, setRegPass] = useState('');
  const [regType, setRegType] = useState('ALUNO');
  const [error, setError] = useState('');
  const [success, setSuccess] = useState('');

  // Banco de Dados - Mantendo apenas o Admin mestre
  const [database, setDatabase] = useState([
    { id: 'ADMIN_001', name: 'Administrador Principal', mail: 'cyber.admin@newwinners.com', pass: 'Nexus99#', type: 'ADMIN', date: '01/01/2024' }
  ]);

  useEffect(() => {
    setError('');
    setSuccess('');
  }, [page]);

  const handleLogin = (e) => {
    e.preventDefault();
    const foundUser = database.find(u => u.mail === email && u.pass === password);

    if (foundUser) {
      setUser(foundUser);
      setPage('dashboard');
    } else {
      setError("Credenciais inválidas. Verifique seu email e senha.");
    }
  };

  const handleRegister = (e) => {
    e.preventDefault();
    
    if (database.some(u => u.mail === regEmail)) {
      setError("Este email já está registrado no sistema.");
      return;
    }

    const newUser = {
      id: Math.random().toString(36).substr(2, 9).toUpperCase(),
      name: regName,
      mail: regEmail,
      pass: regPass,
      type: regType,
      date: new Date().toLocaleDateString()
    };

    setDatabase(prev => [...prev, newUser]);
    setSuccess("Cadastro realizado com sucesso! Redirecionando para o login...");
    
    setTimeout(() => {
      setPage('login');
      setEmail(regEmail);
      // Reset registration form
      setRegName(''); setRegEmail(''); setRegPass('');
    }, 2000);
  };

  const handleLogout = () => {
    setUser(null);
    setEmail('');
    setPassword('');
    setPage('landing');
  };

  // --- COMPONENTES DE INTERFACE ---

  const Sidebar = () => (
    <aside className="w-72 bg-white border-r border-gray-200 flex flex-col p-8">
      <div className="flex items-center space-x-3 mb-12">
         <div className="bg-indigo-600 p-1.5 rounded-lg shadow-md">
           <Globe className="text-white w-5 h-5" />
         </div>
         <span className="font-black text-indigo-900 tracking-tight text-xl">NW PRO</span>
      </div>

      <nav className="flex-1 space-y-2">
        <div className="text-[10px] font-black text-gray-400 uppercase tracking-[0.2em] mb-4 ml-2">Menu Principal</div>
        
        <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl bg-indigo-50 text-indigo-600 font-bold shadow-sm border border-indigo-100">
          <LayoutDashboard className="w-5 h-5" />
          <span>Dashboard</span>
        </button>

        {user?.type === 'ALUNO' && (
          <>
            <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
              <PlayCircle className="w-5 h-5" />
              <span>Minhas Aulas</span>
            </button>
            <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
              <Award className="w-5 h-5" />
              <span>Certificados</span>
            </button>
          </>
        )}

        {user?.type === 'PROFESSOR' && (
          <>
            <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
              <Users className="w-5 h-5" />
              <span>Minhas Turmas</span>
            </button>
            <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
              <FileText className="w-5 h-5" />
              <span>Materiais</span>
            </button>
          </>
        )}

        {(user?.type === 'ADMIN' || user?.type === 'PROFESSOR') && (
          <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
            <Calendar className="w-5 h-5" />
            <span>Agenda</span>
          </button>
        )}

        <button className="flex items-center space-x-3 w-full p-3.5 rounded-xl text-gray-400 hover:bg-gray-50 transition-colors">
          <Settings className="w-5 h-5" />
          <span>Ajustes</span>
        </button>
      </nav>

      <div className="mt-auto p-4 bg-gray-50 rounded-2xl border border-gray-100 mb-6">
        <div className="flex items-center space-x-3">
          <div className={`w-10 h-10 rounded-full flex items-center justify-center font-bold text-white ${user?.type === 'ADMIN' ? 'bg-indigo-600' : user?.type === 'PROFESSOR' ? 'bg-purple-600' : 'bg-blue-600'}`}>
            {user?.name[0]}
          </div>
          <div className="overflow-hidden">
            <p className="text-sm font-bold text-gray-900 truncate">{user?.name}</p>
            <p className="text-[10px] text-gray-500 truncate font-semibold">{user?.type}</p>
          </div>
        </div>
      </div>

      <button onClick={handleLogout} className="flex items-center space-x-3 text-red-400 hover:text-red-600 p-3 font-bold transition-colors">
        <LogOut className="w-5 h-5" />
        <span>Sair do Sistema</span>
      </button>
    </aside>
  );

  const AdminDashboard = () => (
    <div className="space-y-12 animate-in fade-in duration-500">
      <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div className="bg-white p-8 rounded-[2.5rem] border border-gray-100 shadow-sm">
          <div className="w-12 h-12 bg-blue-50 text-blue-500 rounded-2xl flex items-center justify-center mb-6"><GraduationCap /></div>
          <h3 className="text-gray-400 font-bold text-sm uppercase mb-1">Cadastros Totais</h3>
          <p className="text-4xl font-black text-gray-900 tracking-tighter">{database.length}</p>
        </div>
        <div className="bg-white p-8 rounded-[2.5rem] border border-gray-100 shadow-sm">
          <div className="w-12 h-12 bg-purple-50 text-purple-500 rounded-2xl flex items-center justify-center mb-6"><Users /></div>
          <h3 className="text-gray-400 font-bold text-sm uppercase mb-1">Professores</h3>
          <p className="text-4xl font-black text-gray-900 tracking-tighter">{database.filter(u => u.type === 'PROFESSOR').length}</p>
        </div>
        <div className="bg-white p-8 rounded-[2.5rem] border border-gray-100 shadow-sm">
          <div className="w-12 h-12 bg-emerald-50 text-emerald-500 rounded-2xl flex items-center justify-center mb-6"><ShieldCheck /></div>
          <h3 className="text-gray-400 font-bold text-sm uppercase mb-1">Integridade</h3>
          <p className="text-4xl font-black text-gray-900 tracking-tighter">100%</p>
        </div>
      </div>

      <div className="bg-white rounded-[2.5rem] border border-gray-100 shadow-sm overflow-hidden">
        <div className="p-10 border-b border-gray-50 flex justify-between items-center">
          <h3 className="font-black text-gray-900 text-2xl tracking-tight">Base de Dados Central</h3>
        </div>
        <table className="w-full text-left">
          <thead>
            <tr className="bg-gray-50 text-[10px] font-black uppercase tracking-[0.2em] text-gray-400">
              <th className="px-10 py-5">Usuário</th>
              <th className="px-10 py-5">Tipo</th>
              <th className="px-10 py-5 text-right">Data Registro</th>
            </tr>
          </thead>
          <tbody className="divide-y divide-gray-50">
            {database.map(u => (
              <tr key={u.id} className="hover:bg-gray-50/80 transition-all">
                <td className="px-10 py-6">
                  <div className="font-black text-gray-900">{u.name}</div>
                  <div className="text-xs text-gray-400">{u.mail}</div>
                </td>
                <td className="px-10 py-6">
                  <span className={`text-[10px] font-black px-3 py-1 rounded-full ${u.type === 'ADMIN' ? 'bg-indigo-100 text-indigo-600' : u.type === 'PROFESSOR' ? 'bg-purple-100 text-purple-600' : 'bg-blue-100 text-blue-600'}`}>
                    {u.type}
                  </span>
                </td>
                <td className="px-10 py-6 text-right text-xs text-gray-400 font-mono">{u.date}</td>
              </tr>
            ))}
          </tbody>
        </table>
      </div>
    </div>
  );

  const ProfessorDashboard = () => (
    <div className="space-y-8 animate-in slide-in-from-bottom duration-500">
      <div className="bg-indigo-900 text-white p-10 rounded-[2.5rem] relative overflow-hidden shadow-2xl">
        <div className="relative z-10">
          <h2 className="text-3xl font-black mb-2">Hello, Professor {user?.name.split(' ')[0]}!</h2>
          <p className="text-indigo-200">Você tem 3 turmas ativas hoje. Prepare seus materiais.</p>
        </div>
        <div className="absolute top-0 right-0 w-64 h-64 bg-white/10 rounded-full -translate-y-1/2 translate-x-1/3 blur-3xl"></div>
      </div>
      
      <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div className="bg-white p-8 rounded-[2.5rem] border border-gray-100 shadow-sm">
          <h3 className="font-bold text-gray-900 mb-6 flex items-center"><Users className="mr-2 w-5 h-5 text-indigo-500" /> Turmas Ativas</h3>
          <div className="space-y-4">
            {['English Beginners - A1', 'Business English - B2', 'Conversation Club'].map(t => (
              <div key={t} className="flex justify-between items-center p-4 bg-gray-50 rounded-2xl">
                <span className="font-bold text-gray-700">{t}</span>
                <span className="text-xs text-indigo-600 font-bold bg-white px-3 py-1 rounded-lg">Ver Alunos</span>
              </div>
            ))}
          </div>
        </div>
        <div className="bg-white p-8 rounded-[2.5rem] border border-gray-100 shadow-sm">
          <h3 className="font-bold text-gray-900 mb-6 flex items-center"><FileText className="mr-2 w-5 h-5 text-indigo-500" /> Próximas Atividades</h3>
          <div className="space-y-4 text-sm text-gray-500">
            <p>● Correção de redações (Turma A1)</p>
            <p>● Upload de áudio para Listening</p>
            <p>● Planejamento da semana 12</p>
          </div>
        </div>
      </div>
    </div>
  );

  const StudentDashboard = () => (
    <div className="space-y-8 animate-in slide-in-from-bottom duration-500">
      <div className="grid grid-cols-1 md:grid-cols-4 gap-6">
        <div className="bg-white p-6 rounded-3xl border border-gray-100 shadow-sm text-center">
           <div className="text-3xl font-black text-indigo-600 mb-1">85%</div>
           <div className="text-[10px] text-gray-400 font-bold uppercase tracking-widest">Frequência</div>
        </div>
        <div className="bg-white p-6 rounded-3xl border border-gray-100 shadow-sm text-center">
           <div className="text-3xl font-black text-indigo-600 mb-1">B2</div>
           <div className="text-[10px] text-gray-400 font-bold uppercase tracking-widest">Nível Atual</div>
        </div>
        <div className="bg-white p-6 rounded-3xl border border-gray-100 shadow-sm text-center">
           <div className="text-3xl font-black text-indigo-600 mb-1">12</div>
           <div className="text-[10px] text-gray-400 font-bold uppercase tracking-widest">Aulas Concluídas</div>
        </div>
        <div className="bg-white p-6 rounded-3xl border border-gray-100 shadow-sm text-center">
           <div className="text-3xl font-black text-indigo-600 mb-1">4.8</div>
           <div className="text-[10px] text-gray-400 font-bold uppercase tracking-widest">Média Notas</div>
        </div>
      </div>

      <div className="bg-white p-10 rounded-[2.5rem] border border-gray-100 shadow-sm">
        <h3 className="font-black text-gray-900 text-xl mb-8">Continue seu Aprendizado</h3>
        <div className="flex items-center p-6 bg-indigo-50 rounded-[2rem] border border-indigo-100">
          <div className="bg-indigo-600 p-4 rounded-2xl mr-6 text-white"><PlayCircle /></div>
          <div className="flex-1">
            <h4 className="font-black text-indigo-900">Unit 5: Future Continuous</h4>
            <p className="text-indigo-600 text-sm">Aula 12 - Gramática e Conversação</p>
          </div>
          <button className="bg-indigo-600 text-white px-8 py-3 rounded-xl font-bold hover:bg-indigo-700 transition-all">Assistir Agora</button>
        </div>
      </div>

      <div className="bg-white p-10 rounded-[2.5rem] border border-gray-100 shadow-sm">
        <h3 className="font-black text-gray-900 text-xl mb-6">Suas Atividades</h3>
        <div className="space-y-4">
           <div className="flex justify-between items-center p-4 border-b border-gray-50 text-sm">
             <span className="font-bold text-gray-700">Homework 04: Written Expression</span>
             <span className="text-emerald-500 font-bold">Entregue</span>
           </div>
           <div className="flex justify-between items-center p-4 border-b border-gray-50 text-sm">
             <span className="font-bold text-gray-700">Quiz 02: Phrasal Verbs</span>
             <span className="text-red-400 font-bold">Pendente - Expira hoje</span>
           </div>
        </div>
      </div>
    </div>
  );

  // --- LÓGICA DE PÁGINAS ---

  if (page === 'landing') {
    return (
      <div className="min-h-screen bg-[#0a0a0f] text-white selection:bg-indigo-500">
        <nav className="flex justify-between items-center p-6 absolute top-0 w-full z-50">
          <div className="flex items-center space-x-2 cursor-pointer" onClick={() => setPage('landing')}>
            <div className="bg-indigo-600 p-2 rounded-lg shadow-lg shadow-indigo-500/20"><Globe className="text-white w-6 h-6" /></div>
            <span className="text-white font-bold text-xl tracking-tight uppercase">New Winners <span className="text-indigo-400">Pro</span></span>
          </div>
          <div className="space-x-4">
            <button onClick={() => setPage('login')} className="text-gray-300 hover:text-white font-medium">Entrar</button>
            <button onClick={() => setPage('register')} className="bg-white text-indigo-900 px-5 py-2 rounded-full font-bold hover:bg-indigo-50 transition-all shadow-lg">Cadastrar</button>
          </div>
        </nav>
        <main className="flex flex-col items-center justify-center min-h-screen text-center px-4 relative overflow-hidden">
          <div className="absolute top-1/4 -left-20 w-96 h-96 bg-indigo-600/20 rounded-full blur-[120px]"></div>
          <div className="absolute bottom-1/4 -right-20 w-96 h-96 bg-purple-600/20 rounded-full blur-[120px]"></div>
          <div className="z-10 max-w-4xl">
            <h1 className="text-6xl md:text-8xl font-black tracking-tight mb-6 bg-gradient-to-b from-white to-gray-500 bg-clip-text text-transparent">English Mastery.</h1>
            <p className="text-gray-400 text-xl md:text-2xl mb-10 max-w-2xl mx-auto">Plataforma inteligente de gestão educacional para alunos e professores New Winners.</p>
            <button onClick={() => setPage('register')} className="bg-indigo-600 hover:bg-indigo-500 px-10 py-4 rounded-2xl font-bold text-lg transition-all shadow-lg shadow-indigo-600/30">Matricule-se Agora</button>
          </div>
        </main>
      </div>
    );
  }

  if (page === 'login' || page === 'register') {
    return (
      <div className="min-h-screen bg-[#050507] flex items-center justify-center p-4 relative overflow-hidden font-sans">
        <div className="absolute top-10 left-10 z-20">
           <button onClick={() => setPage('landing')} className="text-gray-500 hover:text-white flex items-center transition-colors font-bold uppercase text-xs tracking-widest"><ChevronRight className="rotate-180 mr-2 w-4 h-4" /> Voltar</button>
        </div>
        <div className="w-full max-w-md bg-[#0f0f13] border border-white/5 p-10 rounded-[3rem] shadow-2xl relative z-10">
          <div className="text-center mb-10">
            <div className="inline-flex p-4 bg-indigo-500/10 rounded-2xl border border-indigo-500/20 mb-4 text-indigo-400">
              {page === 'login' ? <LogIn className="w-8 h-8" /> : <UserPlus className="w-8 h-8" />}
            </div>
            <h2 className="text-3xl font-black text-white mb-2">{page === 'login' ? 'Login' : 'Cadastro'}</h2>
            <p className="text-gray-500 text-sm">Portal Acadêmico New Winners</p>
          </div>

          {error && <div className="mb-6 p-4 bg-red-500/10 border border-red-500/20 rounded-xl flex items-center text-red-400 text-xs font-bold"><AlertCircle className="w-4 h-4 mr-2" /> {error}</div>}
          {success && <div className="mb-6 p-4 bg-emerald-500/10 border border-emerald-500/20 rounded-xl flex items-center text-emerald-400 text-xs font-bold"><CheckCircle2 className="w-4 h-4 mr-2" /> {success}</div>}

          <form onSubmit={page === 'login' ? handleLogin : handleRegister} className="space-y-4">
            {page === 'register' && (
              <>
                <input type="text" required value={regName} onChange={(e) => setRegName(e.target.value)} className="w-full bg-black/40 border border-white/5 rounded-xl p-4 text-white focus:ring-1 focus:ring-indigo-500 outline-none" placeholder="Nome Completo" />
                <select value={regType} onChange={(e) => setRegType(e.target.value)} className="w-full bg-black/40 border border-white/5 rounded-xl p-4 text-white focus:ring-1 focus:ring-indigo-500 outline-none font-bold text-xs uppercase tracking-widest">
                  <option value="ALUNO" className="bg-[#0f0f13]">Sou Aluno</option>
                  <option value="PROFESSOR" className="bg-[#0f0f13]">Sou Professor</option>
                </select>
              </>
            )}
            <input type="email" required value={page === 'login' ? email : regEmail} onChange={(e) => page === 'login' ? setEmail(e.target.value) : setRegEmail(e.target.value)} className="w-full bg-black/40 border border-white/5 rounded-xl p-4 text-white focus:ring-1 focus:ring-indigo-500 outline-none" placeholder="Email" />
            <input type="password" required value={page === 'login' ? password : regPass} onChange={(e) => page === 'login' ? setPassword(e.target.value) : setRegPass(e.target.value)} className="w-full bg-black/40 border border-white/5 rounded-xl p-4 text-white focus:ring-1 focus:ring-indigo-500 outline-none" placeholder="Senha" />
            <button className="w-full bg-white text-black font-black py-4 rounded-xl hover:bg-indigo-50 transition-all uppercase text-xs tracking-[0.2em]">{page === 'login' ? 'Acessar' : 'Cadastrar'}</button>
          </form>

          <p className="mt-8 text-center text-gray-500 text-xs font-bold uppercase tracking-widest cursor-pointer" onClick={() => setPage(page === 'login' ? 'register' : 'login')}>
            {page === 'login' ? "Criar nova conta" : "Já tenho conta"}
          </p>
        </div>
      </div>
    );
  }

  return (
    <div className="min-h-screen bg-[#f8f9fc] flex font-sans selection:bg-indigo-100 selection:text-indigo-900">
      <Sidebar />
      <main className="flex-1 p-12 overflow-y-auto">
        <header className="flex justify-between items-end mb-12 animate-in fade-in duration-700">
          <div>
            <h2 className="text-gray-400 font-bold mb-1 uppercase text-[10px] tracking-[0.3em] flex items-center">
              <Clock className="w-3 h-3 mr-2" /> Sessão Ativa: {new Date().toLocaleDateString()}
            </h2>
            <h1 className="text-4xl font-black text-indigo-900 tracking-tight">Portal <span className="text-indigo-400">{user?.type}</span></h1>
          </div>
          <div className="bg-white px-5 py-2.5 rounded-full border border-gray-200 text-[10px] font-black uppercase tracking-widest text-gray-500 shadow-sm">
            Status: <span className="text-emerald-500">Online</span>
          </div>
        </header>

        {user?.type === 'ADMIN' && <AdminDashboard />}
        {user?.type === 'PROFESSOR' && <ProfessorDashboard />}
        {user?.type === 'ALUNO' && <StudentDashboard />}
      </main>
    </div>
  );
};

export default App;
