<script lang="ts">
  import { type Snippet } from 'svelte';

  let { 
    children, 
    variant = 'primary', 
    size = 'md', 
    href = undefined,
    class: className = '',
    ...rest 
  }: { 
    children: Snippet; 
    variant?: 'primary' | 'secondary' | 'ghost' | 'outline' | 'link';
    size?: 'sm' | 'md' | 'lg';
    href?: string;
    class?: string;
    [key: string]: any;
  } = $props();

  const baseStyles = "inline-flex items-center justify-center rounded-md font-medium transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-primary-500 disabled:pointer-events-none disabled:opacity-50";
  
  const variants = {
    primary: "bg-primary-400 text-black hover:bg-primary-300 shadow-sm",
    secondary: "bg-gray-800 text-white hover:bg-gray-700 border border-gray-700",
    ghost: "hover:bg-gray-800 text-gray-300 hover:text-white",
    outline: "border border-gray-700 bg-transparent hover:bg-gray-800 text-gray-300",
    link: "text-primary-400 underline-offset-4 hover:underline"
  };

  const sizes = {
    sm: "h-8 px-3 text-xs",
    md: "h-10 px-4 py-2 text-sm",
    lg: "h-12 px-8 text-base"
  };

  const classes = $derived(`${baseStyles} ${variants[variant]} ${sizes[size]} ${className}`);
</script>

{#if href}
  <a {href} class={classes} {...rest}>
    {@render children()}
  </a>
{:else}
  <button class={classes} {...rest}>
    {@render children()}
  </button>
{/if}
